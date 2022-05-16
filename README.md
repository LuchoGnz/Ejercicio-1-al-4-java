# Ejercicio-1-al-4-java

    System.out.println("Ejercicio N° 1");	
		System.out.println("Los primeros 10 numeros enteros son");
		for (int i = 0; i < 10; i++) {			
		System.out.println(i);
		}
		
		System.out.println("Los primeros 10 numeros pares son");
		
		for (int i = 0; i < 21; i= i + 2) {	
			System.out.println(i);
      
      System.out.println("Ejercicio N° 2 ");
		Scanner ingreso = new Scanner(System.in);
		String[] Palabras = new String[10];
		for (int i = 0; i < 10; i++) {			
			System.out.println("Ingrese la palabra N°" + (i+1));
			Palabras[i] = ingreso.nextLine();
			}
		ingreso.close();
		System.out.println("Las palabras ingresadas mostradas en orden inverso son:");
		for (int i = 9; i >= 0; i--) {
				System.out.println(Palabras[i]);
        
        
    System.out.println("Ejercicio N°3");
		Scanner ingreso2 = new Scanner(System.in);
		String[] Palabras2 = new String [10];
		String textov;
		int ver = 0;
		for (int i = 0; i < 10; i++) {			
			System.out.println("Ingrese la palabra N°" + (i+1));
			Palabras2[i] = ingreso2.nextLine();
			}
		System.out.println("Ingrese la palabra que desea verificar si ya existe:");
		textov = ingreso2.nextLine();
		for (int i = 0; i < 10; i++) {	
			if (Palabras2[i].equals (textov)) {
				System.out.println("El texto ingresado ya existe");
				ver=1;
				}	
			}
				if (ver == 0) { System.out.println("El texto ingresado no existe");
			
		}
		
		ingreso2.close();
    
    
    		System.out.println("Ejercicio N°4");
		ArrayList<Integer> Numeros = new ArrayList<Integer>(); 
		Scanner ingreso3 = new Scanner(System.in);
		int emenor = 0;
		int nro = 0;
		
		System.out.println("Ingrese el entero menor: ");
		emenor = Integer.parseInt(ingreso3.nextLine());
		
		System.out.println("Ingrese los numeros a filtar: ");
		for (int i = 0; i < 20; i++) {			
			System.out.println("Ingreso N°" + (i+1));
			nro = Integer.parseInt(ingreso3.nextLine());
			if (nro > emenor) { Numeros.add(nro);}
			
			}
		
		ingreso3.close();
		
    System.out.println("La lista de numeros mayores a " + emenor + " guardados es: ");
		for (int j = 0; j < (Numeros.size()); j++) {	
		System.out.println(Numeros.get(j)); 
				}
