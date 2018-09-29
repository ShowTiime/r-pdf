	|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|
	|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|
	|-|-|-|-|-|-|SCRIPT CONSTRUCAO E MONTAGEM DE PDF|-|-|-|-|-|-|
	|-|Livro: Sistemas Distribuidos - Conceitos e Projeto - 5e|-|
	|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|
	|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|by - rXs3|-|-|-|
	|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|
	|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|

# Modo de uso

	$ chmod +x r-pdf.sh
	$ ./r-pdf.sh
	
# Observações

Em caso de erros: 'Cache Resources Exhausted', vá até o arquivo policy.xml e altere os resources limits.

	$ cd /etc/ImageMagick-6/
	$ nano policy.xml	#após abrir o arquivo, altere os resources limits.
				#salve e saia.
	
	#verifique se as alterações foram feitas.
	$ convert -list resource
	
	#rode novamente o script
	$ ./r-pdf.sh
