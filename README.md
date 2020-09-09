# OCR_ID
Extração de dados através OCR Imagens (RPA - UiPatch)
Material utilizado (arquivos imagen/excel e a aplicação Identidade.exe) na imersão realizada pela empresa [Desafios RPA](https://desafiosrpa.com.br/) para os inscritos no curso.

## Descrição do Projeto
Ler cada arquivo .png na pasta ID e extrair da imagem as informações Tipo do Documento, ID, Nome e Data de Nascimento, com o Tipo de Documento (PESSOAL ou PROFISSIONAL ou ESTUDANTIL) incluir os demais campos na planilha correspondente, mover cada imagem processada da pasta ID para a pasta Arquivados.
Ler todas as linhas das 3 planilhas (PESSOAL, PROSSIFIONAL e ESTUDANTIL) do arquivo excel Registro.xlsx e incluir as informações na aplicação Identidade.exe, deletando cada linha das planilhas e movendo as informações para o arquivo excel RegistroAll.xlsx para as planilhas correspondentes.

## Detalhamento das Atividades do Robô
  * Ler todas as imagens ID*.png da pasta do projeto ID.
  * Abrir o arquivo de imagem ID*.png.
  * Extrair através de OCR na imagem as informações:
      * Tipo de Documento (Informação ao lado da Identificação -> PESSOAL, PROFISSIONAL e ESTUDANTIL).
      * ID (Informação ao lado de ID:)
      * Nome (Informação ao lado de Nome:)
      * Data Nascimento (Informação ao lado de Nasc.:)
  * Identificar qual a planilha (PESSOAL ou PROFISSIONAL ou ESTUDANTIL) a ser incluído os dados no arquivo excel Registro.xlsx.
  * Montar o registro a ser incluído no arquivo excel Registro.xlsx 
  * Incluir a linha (registro) na planilha correspondente do arquivo excel Registro.xlsx.
  * Fechar o arquivo de imagem ID*.png.
  * Mover o arquivo de imagem ID*.png da pasta ID do projeto para a pasta Arquivados do projeto.
  * Abrir a aplicação Identidade.exe da pasta Identidade do projeto.
  * Ler todas as linhas das três planilhas (PESSOAL, PROFISSIONAL e ESTUDANTIL).
  * Incluir automaticamente as informações na aplicação Identidade.exe onde:
      * Clicar no botão Iniciar.
      * Clicar em Tipo, onde corresponde a planilha sendo lida (PESSOAL, PROFISSIONAL ou ESTUDANTIL).
      * Incluir o ID.
      * Incluir o Nome.
      * Incluir a Data.
      * Clicar no botão Gravar.
  * Incluir a linha lida no arquivo excel RegistroAll.xlsx conforme a planilha que está sendo lida.
  * Deletar a linha lida no arquivo excel Registro.xlsx conforme a planilha que está sendo lida.
  * Enviar uma mensagem a tela "Processo executado com sucesso".
  * Fechar a aplicação Identidade.exe.
  * Encerra a execução do robô.
  
  ### Observações
  Desenvolvido em ambiente Windows 7 Professional, em Sistemas operacionais diferentes, pode ocasionar alguns erros, porem são ajustes simples a serem resolvidos.
