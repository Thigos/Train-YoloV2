# Train-YoloV2

Treine sua IA para detectar objetos com YoloV2 a partir do Google Colab.

Como treinar:
1. Clone o repositório [Darknet](https://github.com/AlexeyAB/darknet)
2. Prepare seu DataSet<br>
  a. Aconselho usar o [LabelImg](https://tzutalin.github.io/labelImg/)
3. Crie duas pastas dentro de darkflow-master/bin, uma para depositar as imagens (```data_image```) e outro para os rótulos(Pascal VOC Data) das imagens (```annotation```)
4. Baixe o [YoloV2-Tiny](https://pjreddie.com/media/files/yolov2-tiny.weights)<br>
  a. Depois do download coloque ele ta nas pasta darkflow-master/bin
5. Configure o ```tiny-yolo-voc.cfg``` de acordo com a [documentação](https://github.com/AlexeyAB/darknet#how-to-train-to-detect-your-custom-objects)<br>
  a. Renomeie o arquivo como ```tiny-yolo-voc-NÚMERODECLASSESc.cfg``` (altere o --model no arquivo ```Train-yolov2.ipynb``` (7° Célula) para o nome do seu .cfg)
6. Faça upload do darflow-master para o Google Drive
7. Execute o arquivo ```Train-yolov2.ipynb``` no Google Colab (Coloque o notebook como GPU para acelerar o treinamento).

Mais informações [aqui](https://github.com/AlexeyAB/darknet/tree/47c7af1cea5bbdedf1184963355e6418cb8b1b4f#how-to-train-pascal-voc-data)

IA Treinada com YoloV2:

![image](https://user-images.githubusercontent.com/67590378/112362271-07a1a200-8cb3-11eb-90e7-de426937fded.png)
