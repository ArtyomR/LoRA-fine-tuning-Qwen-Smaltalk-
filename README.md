# LoRA-fine-tuning-Qwen-Smaltalk-
Задача: **Файн-тюнинг с LoRA**

Теория и пример: https://huggingface.co/learn/llm-course/chapter11/4

Текст задачи: Build on your fine-tuned model from the previous section, but fine-tune it with LoRA. Use the HuggingFaceTB/smoltalk dataset to fine-tune a deepseek-ai/DeepSeek-R1-Distill-Qwen-1.5B model, using the LoRA configuration we defined above.

Был проведён тест с deepseek-ai/DeepSeek-R1-Distill-Qwen-1.5B, но она слишко рассуждающая, задач реализована на модели
Qwen/Qwen2.5-1.5B-Instruct

Реализован пример для Google Colab (1 GPU). Он использует:

* Qwen/Qwen2.5-1.5B-Instruct
* HuggingFaceTB/smoltalk
* LoRA через PEFT
* TRL SFTTrainer

Структура решения:
1. Установка библиотек
2. Авторизация HF (при необходимости)
3. Загрузка модели
4. Настройка LoRA
5. Загрузка датасета
6. Подготовка датасета
7. Обучение LoRA
8. Сохранение адаптера
9. Загрузка базовой модели + LoRA
10. Тестирование и сравнение с базовой моделью
При написании и отладке кода использовался ChatGPT
