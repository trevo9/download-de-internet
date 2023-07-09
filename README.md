# download-de-internet
 importamos a biblioteca speedtest-cli e definimos uma função chamada medir_velocidade_internet(). A biblioteca speedtest-cli nos permite realizar testes de velocidade de internet.


import speedtest

def medir_velocidade_internet():
    # Cria uma instância do Speedtest
    teste = speedtest.Speedtest()

    # Realiza o teste de download
    print("Medindo velocidade de download...")
    velocidade_download = teste.download() / 1000000  # Convertendo para megabits

    # Exibe a velocidade de download
    print("Velocidade de download: %.2f Mbps" % velocidade_download)

medir_velocidade_internet()
