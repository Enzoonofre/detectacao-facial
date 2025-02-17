# Projeto de Detecção e Classificação de Imagens 👤📸🤖

Este projeto tem como objetivo detectar e classificar rostos em imagens utilizando técnicas de visão computacional e aprendizado de máquina. O projeto é dividido em etapas que incluem a detecção de rostos, extração de características (embeddings), treinamento de um modelo de classificação e, finalmente, a classificação de rostos em novas imagens.

## Requisitos 📋

Para executar este projeto, você precisará das seguintes bibliotecas Python:

- `deepface`
- `opencv-python`
- `matplotlib`
- `scikit-learn`
- `numpy`
- `Pillow`

Você pode instalar as dependências necessárias usando o seguinte comando:

```bash
pip install deepface opencv-python matplotlib scikit-learn numpy Pillow
```

## Estrutura do Projeto 🗂️

O projeto é composto por várias etapas, cada uma com um objetivo específico:

1. **Detecção de Rostos** 👤: Utiliza o classificador Haar Cascade para detectar rostos em uma imagem.
2. **Limpeza e Limitação de Imagens** 🧹: Remove imagens corrompidas e limita o número de imagens por categoria.
3. **Extração de Embeddings** 🔍: Utiliza a biblioteca DeepFace para extrair embeddings (vetores de características) das imagens.
4. **Treinamento do Modelo** 🧠: Treina um classificador SVM (Support Vector Machine) utilizando os embeddings extraídos.
5. **Classificação de Rostos** 🎯: Classifica rostos em novas imagens utilizando o modelo treinado.

## Como Executar o Projeto 🚀

1. **Preparação do Ambiente** ⚙️:
   - Certifique-se de que todas as dependências estão instaladas.
   - Monte o Google Drive (se estiver usando o Google Colab) para acessar o dataset de imagens.

2. **Detecção de Rostos** 👤:
   - Execute o código para detectar rostos em uma imagem e exibir os resultados.

3. **Limpeza e Limitação de Imagens** 🧹:
   - Execute o código para limpar imagens corrompidas e limitar o número de imagens por categoria.

4. **Extração de Embeddings** 🔍:
   - Execute o código para extrair embeddings das imagens e salvar os resultados em um arquivo `.pkl`.

5. **Treinamento do Modelo** 🧠:
   - Execute o código para treinar o classificador SVM e salvar o modelo treinado em um arquivo `.pkl`.

6. **Classificação de Rostos** 🎯:
   - Execute o código para classificar rostos em novas imagens e exibir os resultados.

## Exemplo de Uso 🖼️

Aqui está um exemplo de como usar a função `processar_imagem` para classificar rostos em uma imagem:

```python
processar_imagem("pessoas.jpg")
```

Este código irá detectar rostos na imagem `pessoas.jpg`, classificá-los e exibir a imagem com os rostos destacados e os rótulos correspondentes.

## Dataset 📁

O dataset utilizado neste projeto deve estar organizado em pastas, onde cada pasta representa uma categoria (classe) de rostos. Por exemplo:

```
/dataset-rostos
    /Enzo
    /leonard
    /raj
    /sheldon
    /unknown
    /howard
```

Cada pasta deve conter as imagens correspondentes àquela categoria.

## Salvamento de Modelos e Embeddings 💾

Os embeddings extraídos e o modelo treinado são salvos em arquivos `.pkl` para uso futuro:

- `embeddings.pkl`: Contém os embeddings extraídos das imagens.
- `modelo_svm.pkl`: Contém o modelo SVM treinado.

## Considerações Finais 🏁

Este projeto é uma demonstração básica de como detectar e classificar rostos em imagens utilizando técnicas de visão computacional e aprendizado de máquina. Ele pode ser expandido e melhorado de várias maneiras, como a utilização de modelos mais avançados, aumento de dados, e técnicas de otimização.

## Licença 📜

Este projeto está licenciado sob a licença MIT. Consulte o arquivo `LICENSE` para mais detalhes.

## Contato 📧

Para mais informações ou dúvidas, entre em contato com o autor do projeto.

---

**Nota**: Este projeto foi desenvolvido utilizando o Google Colab, mas pode ser adaptado para execução local com algumas modificações.
