[circuit-viewer](https://dirkarnez.github.io/circuit-viewer/)
=============================================================
### TODOs
- [dirkarnez/kicad-symbol-to-svg](https://github.com/dirkarnez/kicad-symbol-to-svg)
- [ ] SVG does not work, during conversion pins' positiion are lost
	- https://dev-docs.kicad.org/en/file-formats/sexpr-schematic/index.html
	- instead, parse `.kicad_sym` directly
  	- https://github.com/theacodes/kicanvas/blob/main/src/viewers/schematic/painter.ts
   	- https://github.com/theacodes/kicanvas/blob/main/src/viewers/schematic/painters/pin.ts
    - ```s
      ...
      (pin passive line
				(at 0 3.81 270)
				(length 1.27)
				(name "~"
					(effects
						(font
							(size 1.27 1.27)
						)
					)
				)
				(number "1"
					(effects
						(font
							(size 1.27 1.27)
						)
					)
				)
			)
			(pin passive line
				(at 0 -3.81 90)
				(length 1.27)
				(name "~"
					(effects
						(font
							(size 1.27 1.27)
						)
					)
				)
				(number "2"
					(effects
						(font
							(size 1.27 1.27)
						)
					)
				)
			)
      ```
