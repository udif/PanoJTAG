This is a KiCAD design (5.99 based) for a voltage level translator that can fit inside the PanoLogic G2. It is intended to develop a cheap JTAG probe by handling the voltage conversion part.
A TX0104B-based design was considered, but abandoned since it has many problems:
* Cannot use in any designs with pullups or pulldowns below 50K
* Max JTAG pin capacitance must be 70pF (which is probably OK, but you need to check that)

Instead, the sn74avc4t774pw was chosen because it used acive drivers with individual direction pins.
The only limitation is that the maximum voltage it can drive is 3.6v which is OK for us.

[3D Render](panojtag.jpg)