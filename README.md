# 🖨️ Integração Java com Impressora Elgin i9
# Sistema de Controle de Impressora Térmica Elgin i9

Aplicação desenvolvida em Java para comunicação e controle de impressoras térmicas Elgin (modelos i8 e i9) utilizando a biblioteca nativa `E1_Impressora01.dll` via JNA. O trabalho faz parte da disciplina de Programação Orientada a Objetos.

## Tecnologias Utilizadas
* **Java 17+** (OpenJDK)
* **IntelliJ IDEA**
* **Biblioteca JNA (`jna-5.15.0.jar`)**
* **DLL Elgin (`E1_Impressora01.dll`)**

## Como Executar o Projeto
1. Abra a pasta raiz do projeto no **IntelliJ IDEA**.
2. Configure o **JDK** em `File -> Project Structure -> Project -> SDK`.
3. Adicione o arquivo `libs Java/jna-5.15.0.jar` em `File -> Project Structure -> Libraries`.
4. Mantenha os arquivos `E1_Impressora01.dll`, `XMLSAT.xml` e `CANC_SAT.xml` na pasta raiz.
5. Execute a classe `Main.java`.

## Credenciais de Acesso (Login)
* **Usuário:** `admin`
* **Senha:** `1234`
*(O sistema permite até 3 tentativas antes de encerrar automaticamente).*

## Funcionalidades do Menu
* **1 - Configurar Conexão:** Define o tipo de comunicação (USB, Serial, Rede, Bluetooth), modelo da impressora, porta e parâmetro.
* **2 - Abrir Conexão:** Inicia a comunicação com a impressora configurada.
* **3 - Fechar Conexão:** Encerra a comunicação ativa com a impressora.
* **4 - Imprimir Texto:** Imprime texto personalizado com opção de múltiplas cópias e corte de papel.
* **5 - Imprimir QR Code:** Gera e imprime um QR Code a partir do conteúdo informado.
* **6 - Imprimir Código de Barras:** Imprime código de barras no padrão Code 128.
* **7 - Imprimir XML SAT:** Lê e imprime o cupom fiscal a partir do arquivo `XMLSAT.xml`.
* **8 - Imprimir XML Cancelamento SAT:** Lê e imprime o comprovante de cancelamento a partir de `CANC_SAT.xml` com assinatura QR Code.
* **9 - Abrir Gaveta:** Envia pulso para abertura da gaveta conectada.
* **10 - Emitir Sinal Sonoro:** Aciona o alerta sonoro (bip) da impressora.
* **11 - Avançar Papel:** Avança a quantidade de linhas informada pelo usuário.
* **0 - Sair:** Fecha a conexão (caso esteja aberta) e encerra o sistema.

## Integrantes do Grupo
Erik Bispo De Sousa
RA:250827
* Erik Bispo de Sousa
* Nome Completo do Integrante 2
