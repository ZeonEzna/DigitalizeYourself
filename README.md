proposed structure:

digital_identity/
│
├── data/
│   ├── audio_raw/           # Nezmenené zvukové nahrávky
│   ├── audio_samples/       # Segmentované hlasové vzorky
│   ├── video_raw/           # Nezmenené video súbory
│   ├── text_corpus/         # SMS, e-maily, dokumenty, chaty
│   ├── questionnaire/       # Výstupy z dotazníkov
│   └── metadata/            # Informácie o osobnosti, veku, dobe, emočný stav atď.
│
├── preprocessing/
│   ├── audio_processing.py  # Čistenie, segmentácia zvuku
│   ├── video_processing.py  # Extrakcia zvuku, analýza výrazu
│   └── text_processing.py   # Tokenizácia, štýlová analýza, NLP extrakcia
│
├── modeling/
│   ├── voice_cloning/       # Tortoise / OpenVoice / Coqui
│   ├── style_embedding/     # Analýza a replikácia komunikačného štýlu
│   └── personality_model/   # Vytváranie jazykovej simulácie osoby (LLM, RAG)
│
├── interface/
│   ├── chat_ui/             # Webová/chatová komunikácia s digitálnou identitou
│   ├── voice_interface/     # Hlasový asistent (text-to-speech + speech-to-text)
│   └── api.py               # Backendová API pre UI a externé volania
│
├── training/
│   ├── train_voice_model.py # Tréning TTS hlasového modelu
│   ├── train_text_model.py  # Tréning štýlového jazykového modelu
│   └── fine_tune_llm.py     # Jemné doladenie veľkého jazykového modelu
│
├── config/
│   ├── paths.yaml           # Cesty k dátam a modelom
│   └── params.yaml          # Hyperparametre, voľby pre trénovanie
│
├── utils/
│   ├── logger.py            # Logovanie udalostí
│   ├── helpers.py           # Pomocné funkcie
│   └── validators.py        # Validácia vstupov a súborov
│
├── main.py                  # Hlavný vstupný bod projektu
└── README.md                # Popis a inštrukcie
