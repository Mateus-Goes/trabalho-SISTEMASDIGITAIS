# Relógio Digital usando VeriLog 

## Descrição do Projeto
Este repositório contém os projetos desenvolvidos na disciplina de Sistemas Digitais do curso de Engenharia de Computação na Escola de Engenharia de São Carlos, Universidade de São Paulo (EESC-USP). Os projetos abrangem a criação de dois tipos de relógios digitais: um utilizando tecnologia TTL (Transistor-Transistor Logic) e outro utilizando tecnologia CMOS (Complementary Metal-Oxide-Semiconductor).

## Estrutura do Repositório
- `Parte1/`: Projetos e documentação relacionados ao relógio digital TTL.
- `Parte2/`: Projetos e documentação relacionados ao relógio digital CMOS.
- `Verilog/`: Código e documentação do contador BCD em Verilog.

## Tecnologias Utilizadas
- **TTL (Transistor-Transistor Logic)**: Utilizamos componentes da família 74LS00 para a construção do relógio digital TTL.
- **CMOS (Complementary Metal-Oxide-Semiconductor)**: Utilizamos componentes da família 4000 para a construção do relógio digital CMOS.
- **Verilog HDL**: Implementação de um contador BCD utilizando Verilog.

## Relógio Digital TTL
### Descrição
O relógio digital TTL foi construído utilizando componentes da família 74LS00. A principal funcionalidade é gerar uma frequência base de 1/60Hz para os contadores do relógio. Utilizamos contadores de década e decodificadores BCD para 7 segmentos para a exibição no display.

### Componentes
- Capacitor 100nF
- Cristal 32,768kHz
- 74HC14
- 74LS90
- 74LS08
- 74LS47
- Displays de 7 segmentos

### Documentação
Para mais detalhes, acesse a documentação completa [aqui](Parte1/RelogioDigitalTTL-TrabalhoSD.pdf).

## Relógio Digital CMOS
### Descrição
O relógio digital CMOS foi construído utilizando componentes da família 4000. Similar ao relógio TTL, ele gera uma frequência base de 1/60Hz para os contadores do relógio, mas utiliza tecnologia CMOS para maior eficiência energética.

### Componentes
- Capacitores (47nF, 20nF, 6,8nF)
- Resistores (10M, 100k)
- Cristal 32,768kHz
- 4518 (Contadores BCD)
- 4049 (Inversor)
- 4081 (Porta AND)
- 4511 (Decodificador BCD para 7 segmentos)
- Displays de 7 segmentos

### Documentação
Para mais detalhes, acesse a documentação completa [aqui](Parte2/RelogioDigitalCMOS.pdf).

## Contador BCD em Verilog
### Descrição
Implementação de um contador BCD (de 000 até 999) utilizando Verilog HDL. Este projeto inclui módulos para contagem de segundos, registradores de 4 bits, e decodificadores de 7 segmentos.

### Arquivos
- `bench.v`: Testbench do contador BCD.
- `model.v`: Modelo do contador BCD.
- `ssd_digit.v`: Decodificador de 7 segmentos.
- `top.v`: Entidade de nível superior que integra todos os módulos.

### Documentação
Para mais detalhes, acesse a documentação completa [aqui](Verilog/TFContadorDigitalVerilog.pdf).

## Como Executar
1. Clone o repositório:
    ```bash
    git clone https://github.com/seu-usuario/seu-repositorio.git
    ```
2. Navegue até o diretório do projeto desejado e siga as instruções específicas de cada projeto contidas na documentação.

## Contribuidores
- Mateus Curtolo de Goes
- Matheus dos Santos Inês
- Matheus Marques dos Santos
- Nicolas Cruz Caldeira
- Olin Medeiros Costa

## Licença
Este projeto está licenciado sob a [MIT License](LICENSE).

