# roadmap:

sooner:
- release python version of models on [fullcontrol website](https://fullcontrol.xyz)
- export 3D mesh of model
    - stl using [VOLCO](https://doi.org/10.1016/j.addma.2018.04.004)
- real time control
- add tutorial info about path length function, circleXY_3pt, catmull_rom, bezier_through_points, interpolated_point, segmented_path
- warn user if they set `line_width` in PlotControls but `style` is not set to 'line' (default = 'tube')
- migrate to pydantic >2.0 - ensure all requirements are met by colab without any dependent package uninstall+reinstall if possible
- investigate: does fc.Point(color= ???) break when calculating colour if not manual colour? What if this is the first point in the list of steps?
- checks to implement before transform()
    - first point in steps has a z value? is this required for sure?
    - first point has color value (if color specified anywhere?) or if color_type = 'manual' in PlotControls


later:
- refactor documentation - [issue](https://github.com/FullControlXYZ/fullcontrol/issues/10)
- update website (www.fullcontrol.xyz) to have more information and have normal website sections? Release website code as open-source repo.
- generalised multi-axis capabilities
- 6-axis robots
- simultaneous control of distributed devices
- collision detection (nozzle/printer-frame/printed-object) - [issue](https://github.com/FullControlXYZ/fullcontrol/issues/21)
- rounded squarewave - [issue](https://github.com/FullControlXYZ/fullcontrol/issues/34)
- show print bed in preview - [issue](https://github.com/FullControlXYZ/fullcontrol/issues/9)
- facilitate 2D plotters (variable line width) - [issue](https://github.com/FullControlXYZ/fullcontrol/issues/15)
- facilitate easy SVG import - [issue](https://github.com/FullControlXYZ/fullcontrol/issues/11)
- allow use of more complex gcode commands like G2/G3 - [issue](https://github.com/FullControlXYZ/fullcontrol/issues/2)
- warn user if centre point has no z value defined - [issue](https://github.com/FullControlXYZ/fullcontrol/issues/36)
- cell control (e.g. dual robots; e.g. printer with supplemental hardware that is not part of the printer)
- area control (e.g. printer farms with microcontrollers)
- factory control (e.g. production line(s))
- enterprise control (e.g. multiple factories)