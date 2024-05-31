
# Título do Projeto

Uma breve descrição sobre o que esse projeto faz e para quem ele é

# System Information Script
Este repositório contém um script Python que utiliza a biblioteca wmi para recuperar e exibir informações básicas do sistema em um computador com Windows.

## Pré-requisitos
Python 3.x
Biblioteca wmi
Você pode instalar a biblioteca wmi utilizando o pip:

bash

```pip install WMI```

## Uso
Clone este repositório ou baixe o arquivo do script.
Certifique-se de que você tenha o Python e a biblioteca wmi instalados.
Execute o script usando um interpretador Python.
bash

python system_info.py

## Descrição do Script
O script recupera e imprime as seguintes informações do sistema:

Fabricante //
Modelo //
Nome //
Número de Processadores //
Tipo de Sistema //
Família do Sistema 

## Exemplo de Saída

Fabricante: [Nome do Fabricante]
Modelo: [Nome do Modelo]
Nome: [Nome do Sistema]
Número de Processadores: [Número de Processadores]
Tipo de Sistema: [Tipo de Sistema]
Família do Sistema: [Família do Sistema]

## Código
Aqui está o código completo do script:

```import wmi
c = wmi.WMI()
my_system = c.Win32_ComputerSystem()[0]

print(f"Manufacturer: {my_system.Manufacturer}")
print(f"Model: {my_system.Model}")
print(f"Name: {my_system.Name}")
print(f"NumberOfProcessors: {my_system.NumberOfProcessors}")
print(f"SystemType: {my_system.SystemType}")
print(f"SystemFamily: {my_system.SystemFamily}")
```


## Licença
Este projeto é licenciado sob a licença MIT. Veja o arquivo LICENSE para mais detalhes.

## Contribuições
Contribuições são bem-vindas! Por favor, abra uma issue ou envie um pull request para quaisquer mudanças.

## Contato
Para quaisquer perguntas ou comentários, por favor entre em contato com [Luccas Pontes] em [luccasxx13@outlook.com].

