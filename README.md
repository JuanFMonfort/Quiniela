# Quiniela
Este es el codigo realizado en Java.
```
  java
```
 
public class Posibilidades {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		int contaVal=0, contaMal=0, conta=0;
		int [] nums= new int[14];
		for (int i = 0; i < 3; i++) { //1
			nums[0]=i;
			for (int j = 0; j < 3; j++) { //2
				nums[1]=j;
				for (int j2 = 0; j2 < 3; j2++) { //3
					nums[2]=j2;
					for (int k = 0; k < 3; k++) { //4
						nums[3]=k;
						for (int k2 = 0; k2 < 3; k2++) { //5
							nums[4]=k2;
							for (int l = 0; l < 3; l++) { //6
								nums[5]=l;
								for (int l2 = 0; l2 < 3; l2++) { //7
									nums[6]=l2;
									for (int m = 0; m < 3; m++) { //8
										nums[7]=m;
										for (int m2 = 0; m2 < 3; m2++) { //9
											nums[8]=m2;
											for (int n = 0; n < 3; n++) { //10
												nums[9]=n;
												for (int n2 = 0; n2 < 3; n2++) { //11
													nums[10]=n2;
													for (int o = 0; o < 3; o++) { //12
														nums[11]=o;
														for (int o2 = 0; o2 < 3; o2++) { //13
															nums[12]=o2;
															for (int p = 0; p < 3; p++) { //14
																nums[13]=p;
																int conta1=0, contaX=0, conta2=0;
																String impresion="";
																for (int q = 0; q < nums.length; q++) {
																	if (nums[q]==0) {
																		impresion=impresion+"1 ";
																		conta1++;
																	}if (nums[q]==1) {
																		impresion=impresion+"X ";
																		contaX++;
																	}if (nums[q]==2) {
																		impresion=impresion+"2 ";
																		conta2++;
																	}
																}
																
																
																if ((conta1>5&&conta1<11)&&(contaX>2&&contaX<6)&&(conta2>3&&conta2<9)) {
																	contaVal++;
																	System.out.println(impresion);
																}else {
																	contaMal++;
																}
																conta++;
																
																
															}//fin 14
														}//fin 13
													}//fin 12
												}//fin 11
											}//fin 10
										}//fin 9
									}//fin 8
								}//fin 7
							}//fin 6
						}//fin 5
					}//fin 4
				}//fin 3
			}//fin 2
		}//fin 1
		System.out.println("\tValidos: "+contaVal);
		System.out.println("\tInvalidos: "+contaMal);
		System.out.println("\tTotales: "+conta);
	}//fin main

}//fin clase
