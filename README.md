# ⚙️ 가상환경 생성 및 활성화  
## 🧠 2-character-chat Project 예시  
OpenAI API + RAG 기반 캐릭터 챗봇 (2기 예시 프로젝트)  
이 프로젝트는 OpenAI API와 RAG(Retrieval-Augmented Generation) 구조를 활용하여 여러 캐릭터가 각각의 개성을 가진 대화를 할 수 있도록 구현한 Flask 기반 챗봇 예제입니다.  

---

## 🧩 프로젝트 클론  
먼저 GitHub 저장소를 클론합니다 👇  
git clone https://github.com/HateSlop/3-chatbot-project-example.git  
cd 3-chatbot-project-example  

---

## ⚙️ 가상환경 생성 및 활성화  

🪟 Windows  
python -m venv hateslop1  
hateslop1\Scripts\activate  

🍎 macOS / Linux  
python3 -m venv hateslop1  
source hateslop1/bin/activate  

---

## 📦 필수 라이브러리 설치  
pip install -r requirements.txt  

---

## 🔑 OpenAI API 키 설정  
1. generation/ 폴더 내부에 .env 파일을 생성  
2. 아래 내용 입력  
OPENAI_API_KEY=sk-xxxxxxxxxxxxxxxxxxxxxxxx  

⚠️ .env 파일은 절대 GitHub에 업로드하지 마세요. (.gitignore에 추가됨)  

---

## 🚀 실행 방법  
python app.py  

콘솔 출력 예시  
* Running on http://127.0.0.1:5000  
👉 브라우저 접속: http://127.0.0.1:5000  

---

## 🧠 주요 기능  
• 캐릭터별 독립 대화 인터페이스 (chatbot1 ~ chatbot5)  
• OpenAI GPT 모델 기반 응답 생성  
• RAG (Retrieval-Augmented Generation) 구조를 활용한 문서 검색  
• .env 파일을 통한 API 키 관리  
• Flask 백엔드 + HTML/CSS/JavaScript 프론트엔드 통합  

---

## 🧰 폴더 구조  
2-character-chat/  
│  
├── app.py — Flask 메인 실행 파일  
├── requirements.txt — 의존성 패키지 목록  
│  
├── generation/ — 캐릭터별 챗봇 로직  
│   ├── chatbot1/  
│   ├── chatbot2/  
│   ├── chatbot3/  
│   ├── chatbot4/  
│   ├── chatbot5/  
│   └── .env — OpenAI API 키 파일  
│  
├── static/ — 정적 파일 (CSS, JS, 이미지, 비디오 등)  
│   ├── css/  
│   ├── js/  
│   └── images/  
│  
└── templates/ — HTML 템플릿 (chat.html 등)  

---

## 🧪 실행 예시  
python app.py  
* Debug mode: on  
* Running on http://127.0.0.1:5000  

브라우저에서 캐릭터 챗봇 인터페이스를 확인할 수 있습니다 🎨  

---

## 🧾 참고사항  
• .env 파일은 보안을 위해 .gitignore에 포함되어 있습니다.  
• 로컬 실행 시 Flask 기본 포트는 5000번입니다.  
• 다른 포트를 사용하려면 app.run(port=5001) 형태로 수정 가능합니다.  
 
