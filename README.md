# QntdAPagarLUZ
Nesse algoritmo apresento um sistema de pagamento de luz por unidade, a cada X unidades o sistema calcula e adiciona um imposto, utilizei a estrutura (SE/SENAO) no Portugol!



programa
 // by Rehfeld13
{
	
	funcao inicio()
	{
	real QntdUsada, ValoraPagar

	escreva ("Informe a quantidade usada: ")
	leia(QntdUsada)

	    	se (QntdUsada <= 50){
	  	ValoraPagar = (QntdUsada * 0.5) * 1.05
	  	escreva ("O valor a ser pago é: "+ValoraPagar)

	  } 	se (QntdUsada > 50 e QntdUsada <= 150){
	  	ValoraPagar = (((QntdUsada - 50) * 0.75) + 25) * 1.05
	  	escreva ("O valor a ser pago é: "+ValoraPagar)
	  	}
	  	se (QntdUsada > 150 e QntdUsada <=250 ){
	  	ValoraPagar = (((QntdUsada - 150) * 1.20) + 100) * 1.05
	  	escreva ("O valor a ser pago é: "+ValoraPagar)
	  	}
	  	senao{
	  	ValoraPagar = (((QntdUsada - 250) * 1.50) + 220) * 1.05
	  	escreva ("O valor a ser pago é: "+ValoraPagar)
	  	}

	
	}
}

