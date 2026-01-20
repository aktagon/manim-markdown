# Prism

Qualified name: `manim.mobject.three\_d.three\_dimensions.Prism`

### *class* Prism(dimensions=[3, 2, 1], \*\*kwargs)

Bases: [`Cube`](manim.mobject.three_d.three_dimensions.Cube.md#manim.mobject.three_d.three_dimensions.Cube)

A right rectangular prism (or rectangular cuboid).
Defined by the length of each side in `[x, y, z]` format.

* **Parameters:**
  * **dimensions** ([*Vector3DLike*](manim.typing.md#manim.typing.Vector3DLike)) – Dimensions of the [`Prism`](#manim.mobject.three_d.three_dimensions.Prism) in `[x, y, z]` format.
  * **kwargs** (*Any*)

### Examples

### Methods

| [`generate_points`](#manim.mobject.three_d.three_dimensions.Prism.generate_points)   | Creates the sides of the [`Prism`](#manim.mobject.three_d.three_dimensions.Prism).   |
|--------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------|

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

#### \_original_\_init_\_(dimensions=[3, 2, 1], \*\*kwargs)

Initialize self.  See help(type(self)) for accurate signature.

* **Parameters:**
  * **dimensions** ([*Vector3DLike*](manim.typing.md#manim.typing.Vector3DLike))
  * **kwargs** (*Any*)
* **Return type:**
  None

#### generate_points()

Creates the sides of the [`Prism`](#manim.mobject.three_d.three_dimensions.Prism).

* **Return type:**
  None
