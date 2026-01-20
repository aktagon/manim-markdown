# Manim Markdown Documentation

Markdown version of the Manim Community Edition documentation for use with AI tools.

## Regenerating the Documentation

```bash
# Clone the manim repository
git clone https://github.com/ManimCommunity/manim.git
cd manim

# Install dependencies
uv sync --group dev
uv add sphinx-markdown-builder --group dev

# Add sphinx_markdown_builder to docs/source/conf.py extensions list:
# "sphinx_markdown_builder",

# Build markdown docs (skip-manim avoids rendering animations)
cd docs/source
uv run sphinx-build -M markdown "." "../build" -t skip-manim

# Copy reference and tutorials
cp -r ../build/markdown/reference ../build/markdown/tutorials /path/to/manim-markdown/
```

## Tutorials

| File | Description |
|------|-------------|
| `tutorials/quickstart.md` | Getting started with Manim |
| `tutorials/building_blocks.md` | Core concepts: Mobjects, Animations, Scenes |
| `tutorials/output_and_config.md` | Rendering and configuration options |

## Reference Manual - Key Classes

### Animations
| Class | File |
|-------|------|
| Animation (base) | `reference/manim.animation.animation.Animation.md` |
| Create / Uncreate | `reference/manim.animation.creation.Create.md` |
| Write / Unwrite | `reference/manim.animation.creation.Write.md` |
| FadeIn / FadeOut | `reference/manim.animation.fading.FadeIn.md` |
| Transform | `reference/manim.animation.transform.Transform.md` |
| ReplacementTransform | `reference/manim.animation.transform.ReplacementTransform.md` |
| MoveAlongPath | `reference/manim.animation.movement.MoveAlongPath.md` |
| Rotate | `reference/manim.animation.rotation.Rotate.md` |
| Indicate | `reference/manim.animation.indication.Indicate.md` |
| AnimationGroup | `reference/manim.animation.composition.AnimationGroup.md` |
| LaggedStart | `reference/manim.animation.composition.LaggedStart.md` |

### Mobjects - Geometry
| Class | File |
|-------|------|
| Mobject (base) | `reference/manim.mobject.mobject.Mobject.md` |
| VMobject | `reference/manim.mobject.types.vectorized_mobject.VMobject.md` |
| VGroup | `reference/manim.mobject.types.vectorized_mobject.VGroup.md` |
| Circle | `reference/manim.mobject.geometry.arc.Circle.md` |
| Dot | `reference/manim.mobject.geometry.arc.Dot.md` |
| Line | `reference/manim.mobject.geometry.line.Line.md` |
| Arrow | `reference/manim.mobject.geometry.line.Arrow.md` |
| Rectangle | `reference/manim.mobject.geometry.polygram.Rectangle.md` |
| Square | `reference/manim.mobject.geometry.polygram.Square.md` |
| Polygon | `reference/manim.mobject.geometry.polygram.Polygon.md` |
| Arc | `reference/manim.mobject.geometry.arc.Arc.md` |

### Mobjects - Text & Math
| Class | File |
|-------|------|
| Text | `reference/manim.mobject.text.text_mobject.Text.md` |
| Tex | `reference/manim.mobject.text.tex_mobject.Tex.md` |
| MathTex | `reference/manim.mobject.text.tex_mobject.MathTex.md` |
| Code | `reference/manim.mobject.text.code_mobject.Code.md` |
| DecimalNumber | `reference/manim.mobject.text.numbers.DecimalNumber.md` |
| Variable | `reference/manim.mobject.text.numbers.Variable.md` |

### Mobjects - Graphing
| Class | File |
|-------|------|
| Axes | `reference/manim.mobject.graphing.coordinate_systems.Axes.md` |
| NumberPlane | `reference/manim.mobject.graphing.coordinate_systems.NumberPlane.md` |
| NumberLine | `reference/manim.mobject.graphing.number_line.NumberLine.md` |
| FunctionGraph | `reference/manim.mobject.graphing.functions.FunctionGraph.md` |
| ParametricFunction | `reference/manim.mobject.graphing.functions.ParametricFunction.md` |
| BarChart | `reference/manim.mobject.graphing.probability.BarChart.md` |

### Mobjects - 3D
| Class | File |
|-------|------|
| ThreeDVMobject | `reference/manim.mobject.three_d.three_dimensions.ThreeDVMobject.md` |
| Sphere | `reference/manim.mobject.three_d.three_dimensions.Sphere.md` |
| Cube | `reference/manim.mobject.three_d.three_dimensions.Cube.md` |
| Cylinder | `reference/manim.mobject.three_d.three_dimensions.Cylinder.md` |
| Arrow3D | `reference/manim.mobject.three_d.three_dimensions.Arrow3D.md` |
| Surface | `reference/manim.mobject.three_d.three_dimensions.Surface.md` |

### Mobjects - Other
| Class | File |
|-------|------|
| Table | `reference/manim.mobject.table.Table.md` |
| Matrix | `reference/manim.mobject.matrix.Matrix.md` |
| Brace | `reference/manim.mobject.svg.brace.Brace.md` |
| SVGMobject | `reference/manim.mobject.svg.svg_mobject.SVGMobject.md` |
| ImageMobject | `reference/manim.mobject.types.image_mobject.ImageMobject.md` |
| ValueTracker | `reference/manim.mobject.value_tracker.ValueTracker.md` |
| Graph | `reference/manim.mobject.graph.Graph.md` |
| VectorField | `reference/manim.mobject.vector_field.VectorField.md` |

### Scenes
| Class | File |
|-------|------|
| Scene | `reference/manim.scene.scene.Scene.md` |
| ThreeDScene | `reference/manim.scene.three_d_scene.ThreeDScene.md` |
| MovingCameraScene | `reference/manim.scene.moving_camera_scene.MovingCameraScene.md` |
| ZoomedScene | `reference/manim.scene.zoomed_scene.ZoomedScene.md` |

### Cameras
| Class | File |
|-------|------|
| Camera | `reference/manim.camera.camera.Camera.md` |
| MovingCamera | `reference/manim.camera.moving_camera.MovingCamera.md` |
| ThreeDCamera | `reference/manim.camera.three_d_camera.ThreeDCamera.md` |

### Utilities
| Module | File |
|--------|------|
| Rate functions | `reference/manim.utils.rate_functions.md` |
| Color | `reference/manim.utils.color.core.ManimColor.md` |
| Bezier | `reference/manim.utils.bezier.md` |
| Space operations | `reference/manim.utils.space_ops.md` |
| Configuration | `reference/manim._config.utils.ManimConfig.md` |
