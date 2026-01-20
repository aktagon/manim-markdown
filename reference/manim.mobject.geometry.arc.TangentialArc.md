# TangentialArc

Qualified name: `manim.mobject.geometry.arc.TangentialArc`

### *class* TangentialArc(line1, line2, radius, corner=(1, 1), \*\*kwargs)

Bases: [`ArcBetweenPoints`](manim.mobject.geometry.arc.ArcBetweenPoints.md#manim.mobject.geometry.arc.ArcBetweenPoints)

Construct an arc that is tangent to two intersecting lines.
You can choose any of the 4 possible corner arcs via the corner tuple.
corner = (s1, s2) where each si is ±1 to control direction along each line.

### Examples

The following example shows all four possible corner configurations:

### Methods

### Attributes

| `animate`             | Used to animate the application of any method of `self`.               |
|-----------------------|------------------------------------------------------------------------|
| `animation_overrides` |                                                                        |
| `color`               |                                                                        |
| `depth`               | The depth of the mobject.                                              |
| `fill_color`          | If there are multiple colors (for gradient) this returns the first one |
| `height`              | The height of the mobject.                                             |
| `n_points_per_curve`  |                                                                        |
| `sheen_factor`        |                                                                        |
| `stroke_color`        |                                                                        |
| `width`               | The width of the mobject.                                              |
* **Parameters:**
  * **line1** ([*Line*](manim.mobject.geometry.line.Line.md#manim.mobject.geometry.line.Line))
  * **line2** ([*Line*](manim.mobject.geometry.line.Line.md#manim.mobject.geometry.line.Line))
  * **radius** (*float*)
  * **corner** (*Any*)
  * **kwargs** (*Any*)

#### \_original_\_init_\_(line1, line2, radius, corner=(1, 1), \*\*kwargs)

Initialize self.  See help(type(self)) for accurate signature.

* **Parameters:**
  * **line1** ([*Line*](manim.mobject.geometry.line.Line.md#manim.mobject.geometry.line.Line))
  * **line2** ([*Line*](manim.mobject.geometry.line.Line.md#manim.mobject.geometry.line.Line))
  * **radius** (*float*)
  * **corner** (*Any*)
  * **kwargs** (*Any*)
