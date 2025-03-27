Algoritmo Tiendita
	Definir Arroz, Yogurt, Avena, ProductoP, CantidadP Como Entero
	Definir PrecioA, InventarioA, PrecioY, CantidadY, PrecioAvena, CantidadAvena Como Entero
	Definir CodigoA, CodigoAvena, CodigoY Como Entero
	Escribir ' ¿Qué producto desea comprar? '
	Escribir ' 1. Arroz '
	// Se le asigna los valores a cada producto
	PrecioA <- 2500
	InventarioA <- 20
	CodigoA <- 1345634
	Escribir ' 2. Yogurt '
	PrecioY <- 800
	InventarioY <- 10
	CodigoY <- 8938384
	Escribir ' 3. Avena '
	PrecioAvena <- 1600
	InventarioAvena <- 30
	CodigoAvena <- 839234
	Repetir
		Leer ProductoP
		Si ProductoP==1 Entonces
			Escribir ' El precio del arroz es de: ', PrecioA
			Escribir ' Hay ', InventarioA, ' libras de Arroz '
			Escribir ' El código del arroz es: ', CodigoA
			Escribir ' ¿Qué cantidad quiere comprar? '
			Repetir
				Leer CantidadP
				Si CantidadP>InventarioA Entonces
					Escribir ' No hay suficiente Arroz '
				FinSi
			Hasta Que CantidadP<=InventarioA
			InventarioA <- InventarioA-CantidadP
			Escribir ' Quedan ', InventarioA, ' libras de arroz '
			Si InventarioA<=5 Entonces
				Escribir ' Debe surtir arroz '
			FinSi
		FinSi
		Si ProductoP==2 Entonces
			Escribir ' El precio del yogurt es de: ', PrecioY
			Escribir ' Hay ', InventarioY, ' yogures '
			Escribir ' El código del yogurt es: ', CodigoY
			Escribir ' ¿Qué cantidad quiere comprar? '
			Repetir
				Leer CantidadP
				Si CantidadP>InventarioY Entonces
					Escribir ' No hay suficiente Yogurt '
				FinSi
			Hasta Que CantidadP<=InventarioY
			InventarioY <- InventarioY-CantidadP
			Escribir ' Quedan ', InventarioY, ' yogures '
			Si InventarioY<=4 Entonces
				Escribir ' Debe surtir yogurt '
			FinSi
		FinSi
		Si ProductoP==3 Entonces
			Escribir ' El precio de la avena es de: ', PrecioAvena
			Escribir ' Hay ', InventarioAvena, ' Avenas '
			Escribir ' El código de la avena es: ', CodigoY
			Escribir ' ¿Qué cantidad quiere comprar? '
			Repetir
				Leer CantidadP
				Si CantidadP>InventarioAvena Entonces
					Escribir ' No hay suficiente Avena '
				FinSi
			Hasta Que CantidadP<=InventarioAvena
			InventarioAvena <- InventarioAvena-CantidadP
			Escribir ' Quedan ', InventarioAvena, ' Avenas '
			Si InventarioAvena<=8 Entonces
				Escribir ' Debe surtir Avena '
			FinSi
		SiNo
			Escribir 'Seleccione un producto de la lista'
		FinSi
	Hasta Que ProductoP==1 O ProductoP==2 O ProductoP==3
FinAlgoritmo
