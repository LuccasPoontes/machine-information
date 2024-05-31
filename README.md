# machine-information
O código fornecido utiliza a biblioteca wmi para acessar informações sobre o sistema do computador.

Importação da Biblioteca WMI:

python
Copiar código
import wmi
Esta linha importa a biblioteca wmi, que é uma interface para o Windows Management Instrumentation. Esta biblioteca permite que você acesse e manipule informações de gerenciamento e configurações do Windows.

Instanciação do Objeto WMI:

python
Copiar código
c = wmi.WMI()
Aqui, um objeto WMI é criado. Este objeto é usado para interagir com o sistema WMI do Windows.

Recuperação de Informações do Sistema:

python
Copiar código
my_system = c.Win32_ComputerSystem()[0]
Esta linha obtém uma lista de objetos Win32_ComputerSystem, que contém informações sobre o sistema do computador. O índice [0] é usado para acessar o primeiro (e geralmente o único) objeto nesta lista, representando o computador atual.

Impressão das Informações do Sistema:
O código a seguir imprime várias informações sobre o sistema:

python
Copiar código
print(f"Manufacturer: {my_system.Manufacturer}")
print(f"Model: {my_system.Model}")
print(f"Name: {my_system.Name}")
print(f"NumberOfProcessors: {my_system.NumberOfProcessors}")
print(f"SystemType: {my_system.SystemType}")
print(f"SystemFamily: {my_system.SystemFamily}")
Estas linhas usam formatação de strings para exibir as seguintes informações:

Manufacturer: O fabricante do sistema (por exemplo, Dell, HP, etc.).
Model: O modelo do sistema.
Name: O nome do sistema.
NumberOfProcessors: O número de processadores no sistema.
SystemType: O tipo de sistema (por exemplo, x64-based PC).
SystemFamily: A família do sistema (por exemplo, família de computadores desktop ou laptop).
