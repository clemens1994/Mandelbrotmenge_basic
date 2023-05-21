10 INPUT "Real and imaginary part that marks the lower left corner? (seperated with ",")"; Rmin, Imin
20 INPUT "Sidelength of the cutout?"; K
30 INPUT "Number of iterations in every point?"; ITmax
40 Schrittweite = K/400
50 R = Rmin
60 FOR S = 1 TO 400 STEP 1
70 	I = Imin
80 	FOR Z = 400 TO 1 STEP -1
90		IT = 0
100		X = 0
110		Y = 0
120		WHILE IT <= ITmax AND SQR(X^2+Y^2)<2
130			IT = IT + 1
140			Xu = X
150			X = X^2-Y^2 + R
160			Y = 2*Xu*Y + I
170		WEND
180		SCREEN 12
190	IF IT >= ITmax THEN PSET (S,Z)
200	I = I + Schrittweite
210	NEXT Z
220 R = R + Schrittweite
230 NEXT S
