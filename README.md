<img width="4829" height="1339" alt="1" src="https://github.com/user-attachments/assets/ab48bb68-8a1f-4ffc-8059-83680e12ee01" />
<img width="4829" height="2572" alt="2" src="https://github.com/user-attachments/assets/1cb50aef-7959-46b9-ab80-e1080267d149" />

```python
class ML_Developer:
    name        = "Mederbek"
    experience  = "24 months"
    focus       = "ML Engineering"
    interest    = ["Agentic AI Engineer", "Research Engineer", "Post-Training & Reasoning", "Alignment & AI Safety"]
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

    AI Agent Engineer:
    junior = {
    "llm_basics":    ["OpenAI API / Claude SDK", "Sampling (temperature, top-k, top-p)"],
    "prompting":     ["Few-shot / Chain-of-Thought", "Structured output (JSON mode)", "System prompt design"],
    "agents_core":   ["Tool Calling", "LangGraph базовый (простые графы)"],
    "rag_basics":    ["Embeddings концептуально", "Qdrant/pgvector — базовый поиск", "Chunking стратегии"],
    "context":       ["Sliding window", "Token budget — считать примерно"],
    }
    middle = {
    "agents_advanced": ["MCP", "Мульти-агентные графы (LangGraph)", "Error handling / retry для tool calls"],
    "rag_advanced":    ["Hybrid Search (BM25 + vector)", "Reranking (cross-encoder)", "Fine-tune embeddings под домен"],
    "context_deep":    ["Суммаризация истории диалога", "Token budget management (точный расчёт)"],
    "evaluation":      ["LangSmith", "Ragas", "Тестирование промптов"],
    "llm_testing":     ["Mocking LLM-ответов в pytest", "Snapshot-тесты для RAG"],
    "streaming":       ["SSE/WebSocket токенов", "Связка с своим стеком (Channels)"],
    "caching":         ["Semantic caching"],
    "cost_tracking":   ["Token usage monitoring", "Cost per request"],
    "finetuning_light":["Instruction Tuning / SFT — понимать когда нужен"],
    }
    senior = {
    "finetuning":      ["SFT практически", "RLHF/DPO концептуально", "Dataset preparation"],
    "alignment":       ["RLHF (reward model, PPO)", "Constitutional AI", "Prompt injection — атака и защита глубоко"],
    "optimization":    ["vLLM", "AWQ/GPTQ/GGUF квантование", "KV-cache, batching"],
    "mlops":           ["MLflow", "Drift Monitoring"],
    "observability":   ["OpenTelemetry", "Prometheus + Grafana"],
    "security":        ["OAuth2 PKCE", "Rate Limiting паттерны", "Prompt Injection защита — production-grade"],
    "async_infra":     ["RabbitMQ/Celery — тяжёлые фоновые пайплайны", "Airflow — если MLOps плотно"],
    "architecture":    ["Проектирование multi-agent систем с нуля", "Trade-offs: latency vs cost vs quality"],
    }
```
