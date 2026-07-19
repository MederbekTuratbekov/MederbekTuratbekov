<img width="4829" height="1339" alt="1" src="https://github.com/user-attachments/assets/ab48bb68-8a1f-4ffc-8059-83680e12ee01" />
<img width="4829" height="2572" alt="2" src="https://github.com/user-attachments/assets/1cb50aef-7959-46b9-ab80-e1080267d149" />

```python
class ML_Developer:
    name        = "Neo"
    experience  = "24 months"
    focus       = "ML Engineering"
    interest    = ["Research Engineer", "Post-Training & Reasoning", "Alignment & AI Safety"]
    principles  = ["DRY", "KISS", "SOLID"]
    goal        = "AGI Engineer"

    stack = {
        "backend":      ["Python", "FastAPI", "Django", "Django Templates", "DRF", "Django Channels", "Pydantic", "SQLAlchemy", "Alembic", "sqladmin"],
        "ml_ai":        ["PyTorch", "Scikit-learn", "OpenCV", "YOLO", "NumPy", "Pandas", "Matplotlib", "Seaborn", "RoboFlow"],
        "platforms":    ["Google Colab", "Kaggle", "Hugging Face", "n8n"],
        "databases":    ["PostgreSQL", "MySQL", "Redis"],
        "devops":       ["Linux", "Docker", "NGINX", "AWS", "Gunicorn", "Uvicorn", "Daphne", "Git", "GitHub", "Postman"],
        "api":          ["REST", "GraphQL", "WebSocket", "gRPC", "SOAP", "HTTP/2", "CORS"],
        "architecture": ["Monolith", "Microservices", "n8n"],
        "libraries":    ["Alembic", "Joblib", "Pillow", "pytest", "Authlib", "passlib", "Streamlit"],
    }

    ml_deep_dive = {
        "audio_ml":           ["torchaudio", "MelSpectrogram", "AmplitudeToDB", "Resample (сэмплрейт нормализация)", "soundfile"],
        "nlp":                ["torchtext", "LSTM", "BiLSTM", "nn.Embedding", "CountVectorizer", "Naive Bayes (MultinomialNB)", "build_vocab_from_iterator", "HuggingFace datasets"],
        "cnn_architectures":  ["Conv2d/MaxPool2d/AdaptiveAvgPool2d", "BatchNorm2d", "Dropout2d", "VGG-style blocks", "transfer learning patterns"],
        "classic_ml":         ["LogisticRegression", "DecisionTree", "RandomForest", "XGBoost", "SVC", "KNeighborsClassifier"],
        "ml_techniques":      ["class_weight='balanced' (дисбаланс классов)", "stratify (стратифицированное разбиение)", "CosineAnnealingLR / StepLR (scheduler)", "label_smoothing", "collate_fn (кастомный батчинг)", "AdaptiveAvgPool2d (переменная длина входа)"],
        "metrics":            ["accuracy", "F1", "ROC-AUC", "R²", "precision/recall", "classification_report"],
    }

    learning = {
        "classical_ml_gaps":  ["MLP с нуля (forward/backward руками)", "Transfer Learning (дообучение ResNet/EfficientNet под задачу)", "Mixed Precision Training (fp16/bf16, torch.cuda.amp)"],  # 0. ФУНДАМЕНТ — LoRA и fine-tuning не будут "магией"
        "transformers_core_from_scratch": ["Self-Attention, Multi-Head Attention", "Positional Encoding", "Encoder / Decoder архитектура", "Реализовать GPT-mini с нуля"], # 01. ОСНОВА
        "transformers_tools": ["HuggingFace Transformers", "PEFT / LoRA", "Tokenizers"],                                                                                   # 02. ИНСТРУМЕНТЫ — теперь понимаешь что под капотом
        "llm_entry":          ["OpenAI API", "Claude SDK", "LangChain"],                                                                                                   # 03. LLM ВХОД — подключение к реальным моделям
        "text_generation":    ["Sampling стратегии (temperature, top-k, top-p)", "Beam search", "Constrained/structured generation"],                                      # 04. ГЕНЕРАЦИЯ — как модель реально выбирает следующий токен
        "prompt_engineering": ["Few-shot / Chain-of-Thought", "Structured output (JSON mode)", "System prompt design"],                                                    # 05. ПРОМПТИНГ — отдельный навык, не "само собой"
        "embeddings":         ["Как выбрать embedding-модель", "Dimension, cosine vs dot product", "Fine-tune embeddings под домен"],                                      # 06. EMBEDDINGS — фундамент RAG, без этого поиск "работает как повезёт"
        "rag":                ["Qdrant", "pgvector", "Hybrid Search", "BM25", "Chunking стратегии", "Reranking (Cohere / cross-encoder)"],                                 # 07. RAG — хранение и поиск знаний
        "agents":             ["Tool Calling", "LangGraph", "MCP"],                                                                                                        # 08. АГЕНТЫ — LLM начинает действовать
        "context_management": ["Sliding window", "Суммаризация истории диалога", "Token budget management"],                                                               # 09. КОНТЕКСТ — без этого агенты упрутся в лимит токенов
        "multimodal":         ["Vision-Language модели (CLIP, GPT-4V-стиль)", "Связка YOLO/OpenCV опыта с LLM"],                                                           # 10. МУЛЬТИМОДАЛЬНОСТЬ — твоё преимущество, раз уже знаешь CV
        "diffusion":          ["Stable Diffusion концептуально (forward/reverse process)", "Text-to-image / text-to-audio генерация", "ComfyUI или diffusers basics"],     # 11. ДИФФУЗИЯ — отдельный класс генеративных моделей, не transformer-based. (Stable Diffusion — отдельная экосистема. Оставь как "читал, понимаю концепт", не трать время на глубину.)
        "evaluation":         ["LangSmith", "Ragas", "TruLens"],                                                                                                           # 12. ОЦЕНКА — без этого не знаешь работает ли система
        "finetuning":         ["Instruction Tuning / SFT", "RLHF / DPO концептуально", "Dataset preparation для fine-tune"],                                               # 13. FINE-TUNING — когда промпта уже мало
        "alignment_basics":   ["RLHF концептуально (reward model, PPO)", "Constitutional AI (как работает Anthropic)", "Jailbreaks и prompt injection — не только защита, но и понимание природы"],  # 13.5. ALIGNMENT — без этого не пройти интервью в Anthropic/OpenAI; они спрашивают это даже на инженерных позициях
        "streaming":          ["SSE / WebSocket стриминг токенов", "Связка с Django Channels из твоего стека"],                                                            # 14. СТРИМИНГ — юзер не ждёт весь ответ разом
        "llm_testing":        ["Mocking LLM-ответов в pytest", "Snapshot-тесты для RAG", "Тестирование промптов"],                                                         # 15. ТЕСТИРОВАНИЕ — отдельная дисциплина, не обычный unit-test
        "caching":            ["Semantic caching (кэш по смыслу, не по строке)", "Связка с Redis из твоего стека"],                                                        # 16. КЭШИРОВАНИЕ — не платить дважды за один и тот же смысл вопроса
        "cost_tracking":      ["Token usage monitoring", "Cost per request tracking"],                                                                                     # 17. СТОИМОСТЬ — первое, что спросит product-интервьюер
        "async_infra":        ["RabbitMQ", "Celery", "Airflow"],                                                                                                           # 18. ОЧЕРЕДЬ И ФОНОВЫЕ ЗАДАЧИ (Celery для старта, Airflow только если займёшься MLOps плотно)
        "mlops":              ["MLflow", "Drift Monitoring"],                                                                                                              # 19. MLOPS — трекинг экспериментов и мониторинг дрейфа
        "optimization":       ["vLLM", "AWQ / GPTQ / GGUF", "KV-cache, batching, quantization на пальцах"],                                                                # 20. ОПТИМИЗАЦИЯ — когда модель уже работает
        "observability":      ["OpenTelemetry", "Prometheus + Grafana"],                                                                                                   # 21. НАБЛЮДАЕМОСТЬ — production-готовность (достаточно знать что это есть и уметь читать дашборды)
        "security":           ["JWT глубоко", "OAuth2 PKCE", "Rate Limiting паттерны", "Prompt Injection защита"],                                                         # 22. БЕЗОПАСНОСТЬ — для LLM отдельный класс атак
    }
```
