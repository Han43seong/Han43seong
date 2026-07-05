## 김한성 (Han43seong)

**폐쇄망 RAG 시스템을 설계하고, 코딩 에이전트 주도 개발과 자동 검증으로 완성까지 책임지는 개발자**
Closed-network RAG systems — designed by me, built with coding agents, proven by automated verification.

방산·IPS 기업 재직 (2024.04~). 외부망이 차단된 환경이 기본 전제입니다.
설계와 검증 기준은 직접 잡고, 구현은 에이전트를 지휘하며, 결과는 자동 QA 루프로 증명합니다.

<!-- TODO: 데모 영상 촬영 후 여기에 삽입 — 비행기 모드 태블릿에서 RAG가 동작하는 90초 영상 GIF/링크 -->

### 숫자로 보는 작업

- 🔒 S1000D 기술문서 RAG — PC 파이프라인부터 Android 온디바이스 앱까지 **완전 오프라인**
- ✅ **500케이스 자동 QA→수정→재검증 루프 500/500 통과** — 실패 3건은 루프가 자동 수정 ([검증 리포트](https://github.com/Han43seong/S1000D-RAG/blob/main/docs/rag_quality_evidence_report.md))
- ⏱️ 온디바이스 LLM 응답 **30초+ → 10초대** 단축 (실무 프로토타입, 고객 시연까지 진행)
- 📝 실패도 기록합니다 — [v1 실패 분석](https://github.com/Han43seong/S1000D-RAG/blob/main/docs/retrospectives/rag-v1-failure-analysis.md) → [v4 재설계 회고](https://github.com/Han43seong/S1000D-RAG/blob/main/docs/retrospectives/rag-evolution-v1-to-v4.md)

### 대표 프로젝트

| 프로젝트 | 한 줄 |
|---|---|
| [**S1000D-RAG**](https://github.com/Han43seong/S1000D-RAG) | 폐쇄망 기술문서 질의응답 RAG — 온톨로지가 검색을 통제하고, 근거가 부족하면 LLM 생성을 차단 |
| [**S1000D-RAG-Android**](https://github.com/Han43seong/S1000D-RAG-Android) | 완전 오프라인 온디바이스 RAG 앱 — ONNX int8 임베딩 + llama.cpp, Galaxy Tab 실기기 동작 |
| [**just-chill**](https://github.com/Han43seong/just-chill) | 코딩 에이전트의 "완료" 보고를 근거(변경 내역·테스트 결과)로 검증하는 정책 레이어 |

### Stack

`Python` `Kotlin` `ChromaDB` `bge-m3` `bge-reranker-v2-m3` `rdflib (RDF/OWL·SPARQL)` `llama.cpp` `ONNX Runtime Mobile` `whisper.cpp` `FastAPI` `Jetpack Compose` `Room` `Docker` `Gitea CI`

**개발 방식** — Claude Code·Codex·Gemini 멀티모델 오케스트레이션 + 자동 검증 하네스. 완료는 로그가 아니라 테스트 결과로 판단합니다.

📫 han43seong@gmail.com
