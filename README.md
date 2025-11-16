# 🧠 Trabalho 2 – Redes Neurais  
## Classificação de Lixo para Reciclagem (TrashNet)

Este projeto implementa um classificador de imagens multiclasse utilizando Redes Neurais Convolucionais (CNN) para auxiliar no processo de triagem de resíduos recicláveis — um tema alinhado com os desafios atuais de sustentabilidade e foco da COP 30.  
O objetivo é classificar imagens de lixo em uma das seis categorias do dataset **TrashNet**:

- **glass** (vidro)  
- **paper** (papel)  
- **cardboard** (papelão)  
- **plastic** (plástico)  
- **metal** (metal)  
- **trash** (rejeito / lixo orgânico)

---

# 📊 Resultados

## ✔️ Curva de Acurácia  
Mostra a evolução da acurácia de treino e teste ao longo das 20 épocas:

![accuracy](nb_images/cell_28_image.png)

📌 **Observações:**  
- Acurácia de treino estabiliza próximo de **0.57**  
- Acurácia de validação fica em torno de **0.51**  
- Indícios de leve overfitting, porém esperado em datasets pequenos

---

## 🧱 Matriz de Confusão

A matriz abaixo mostra como o modelo acertou ou confundiu as classes:

![confusion-matrix](nb_images/cell_33_image.png)

### Principais observações:
- A classe **glass** foi a mais bem reconhecida (48 acertos)
- Classes como **trash** e **cardboard** têm mais confusões  
- As classes visualmente parecidas (ex.: *paper*, *plastic* e *cardboard*) geram mais erros

---

# 📌 Métricas

- **Acurácia de treino:** ~57%  
- **Acurácia de teste:** ~51%  
- **Percepção geral:** modelo inicial razoável para dataset pequeno  
- Data augmentation melhorou estabilidade do aprendizado  

---

