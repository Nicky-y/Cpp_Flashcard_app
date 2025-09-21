# Cpp_Flashcard_app
A GUI flashcard app with a C++ problems
<img width="1920" height="899" alt="Cpp_flashcard_app" src="https://github.com/user-attachments/assets/2bd0d6f6-fccb-4004-8bea-4bea66c8a4c2" />
<img width="1920" height="896" alt="Cpp_flashcard_app_2" src="https://github.com/user-attachments/assets/4de58772-babe-4e0e-ad21-45b578c40d79" />
<img width="1920" height="892" alt="Cpp_flashcard_app_3" src="https://github.com/user-attachments/assets/bc066e07-88b6-47b1-a154-1afce397ce5f" />

Architecture:

cpp-flashcards/
├─ CMakeLists.txt
├─ third_party/            # (Option: nlohmann/json, sqlite3, raylib, drogon)
├─ core/
│  ├─ CMakeLists.txt
│  ├─ model/
│  │  ├─ Card.h
│  │  └─ CardTypes.h
│  ├─ sr/
│  │  └─ SpacedRepetition.h
│  ├─ judge/
│  │  ├─ IValidator.h
│  │  ├─ TokenValidator.h
│  │  ├─ OutputCompare.h
│  │  ├─ IRunner.h
│  │  └─ LocalRunner.h
│  └─ storage/
│     ├─ IRepository.h
│     ├─ JsonRepo.h
│     └─ SqliteRepo.h
├─ apps/
│  ├─ gui_raylib/
│  │  ├─ CMakeLists.txt
│  │  └─ main.cpp
│  └─ server_drogon/        # (Option)
│     ├─ CMakeLists.txt
│     └─ main.cpp
└─ data/
   └─ deck_example.json 
