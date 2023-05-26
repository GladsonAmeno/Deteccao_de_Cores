# Detecção de Cores com OpenCV

Este projeto demonstra a detecção de cores utilizando a biblioteca OpenCV em Python. Através da câmera, o programa é capaz de identificar objetos em tempo real com base em seus intervalos de cores definidos.

## Funcionalidade

O programa realiza as seguintes etapas:

1. Inicializa a webcam para capturar o vídeo em tempo real.
2. Define um dicionário de cores e seus respectivos limites de intervalo no espaço de cores HSV.
3. Pré-processa cada quadro de vídeo capturado, redimensionando e aplicando suavização para reduzir ruídos.
4. Converte o quadro para o espaço de cores HSV.
5. Itera sobre cada cor definida no dicionário.
6. Cria uma máscara para a cor atual com base nos limites definidos.
7. Aplica operações morfológicas para melhorar a forma dos objetos detectados na máscara.
8. Encontra os contornos dos objetos detectados na máscara.
9. Verifica se pelo menos um contorno foi encontrado e, se sim, encontra o maior contorno.
10. Verifica a área do contorno para filtrar pequenos ruídos.
11. Desenha um retângulo em volta do objeto detectado e escreve o nome da cor no retângulo.
12. Exibe o quadro com as detecções em uma janela.
13. O loop continua até que a tecla 'q' seja pressionada para encerrar o programa.

## Pré-requisitos

- Python 3.x
- Biblioteca OpenCV (opencv-python) -> pip install opencv-python

## Como executar o programa

1. Certifique-se de ter o Python instalado no seu sistema.
2. Instale a biblioteca OpenCV executando o seguinte comando: pip install opencv-python
3. Clone ou faça o download deste repositório para o seu computador.
4. Navegue até o diretório do projeto no seu terminal.
5. Execute o seguinte comando: python main.py
6. Uma janela será aberta, exibindo o vídeo da webcam com as detecções de cores em tempo real.
7. Pressione a tecla 'q' para encerrar o programa.

## Contribuição

Contribuições são bem-vindas! Se você deseja adicionar novas funcionalidades, corrigir bugs ou melhorar este projeto de alguma forma, fique à vontade para abrir um pull request.

## Licença

Este projeto está licenciado sob a [Licença MIT](LICENSE).


