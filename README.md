# Suspicious Traffic Analytics 🚨

ML-based malware detection в сетевом трафике на реальных PCAP данных.

## 📊 Данные
- **Источник**: [ActiveCM Threat Hunting Labs](https://activecm.github.io/threat-hunting-labs/)
- **Размер**: ~1GB (2 CSV файла)
- **Задача**: Обнаружение вредоносного трафика (binary classification)

## 🛠️ Что сделано
1. **Предобработка**: timestamps → datetime, заполнение пропусков
2. **Признаки**: длина пакетов, частота запросов, подозрительные домены, ночная активность
3. **Балансировка**: SMOTE
4. **Модели**: Logistic Regression, LinearSVC, Ridge, GaussianNB, Decision Tree

## 📈 Результаты

| Модель             | Accuracy | Precision | Recall | F1     |
|--------------------|----------|-----------|--------|--------|
| Decision Tree      | **0.9997**| **1.00**  | **1.00**| **1.00**|
| Ridge Classifier   | **0.9780**| **0.96**  | **1.00**| **0.98**|
| LinearSVC          | 0.8422   | 0.83      | 0.86   | 0.84   |

## 🖥️ Стек
Python - pandas - scikit-learn - SMOTE - matplotlib

text

## 📄 Отчёт
[FINAL-PROJECT-REPORT.pdf](FINAL-PROJECT-REPORT.pdf)

**Pet проект** • Cybersecurity • Machine Learning
