# 📰 한 주 요약
매주 커뮤니티 리뷰를 거친, 이번 주 가장 가치있는 소식 모음입니다.
매주 수요일 업데이트 됩니다.
## 📆 [2025/06/16 ~ 2025/06/22] 주간 소식
## ⭐ 4점

### 1. Anthropic의 멀티 에이전트 기반 연구 시스템: 아키텍처, 설계 전략, 성능 최적화
요약 없음

> **Why it matters:** 
> 내용 없음

### 2. 멀티모달 대형 언어모델이 집으로 가는 길을 안내할 수 있을까? 교통지도 기반 세밀한 시각적 추론 평가를 위한 벤치마크 연구 / Can MLLMs Guide Me Home? A Benchmark Study on Fine-Grained Visual Reasoning from Transit Maps
ReasonMap은 세밀한 시각적 추론 능력을 평가하기 위해 고해상도 교통 지도를 기반으로 만든 MLLM 벤치마크로, 기존 모델들의 시각적 추론 성능과 오픈소스/폐쇄형 모델 간 성능 차이를 드러낸다

> **Why it matters:** 
> 시각적 추론 능력은 멀티모달 AI의 핵심 과제이며, ReasonMap은 그동안 간과되었던 ‘정밀한 공간 추론’ 능력을 정량적으로 평가할 수 있는 첫 체계적 시도 중 하나로, MLLM의 한계와 발전 방향을 동시에 보여주기 때문이다.

### 3. Text-to-LoRA (T2L): A Hypernetwork that Generates Task-Specific LLM Adapters (LoRAs) based on a Text Description of the Task
	1.	Sakana AI의 Text-to-LoRA(T2L)는 자연어 설명만으로 LLM용 LoRA 어댑터를 자동 생성하는 기술입니다.
2.	별도의 훈련 없이 텍스트 입력만으로 다양한 작업에 맞는 어댑터를 즉시 만들 수 있습니다.
3.	기존 수동 방식과 비슷하거나 더 나은 성능을 보여, LLM 커스터마이징이 훨씬 쉬워졌습니다.

> **Why it matters:** 
> 기존에 많은 학습 리소스가 필요한 LoRA를 자연어 명령어로 zero-shot 업데이트를 할 수 있습니다

### 4. Why agents are bad pair programmers
LLM agents make bad pairs because they code faster than humans think.
1. throttle down from the semi-autonomous "Agent" mode to the turn-based "Edit" or "Ask" modes (자율적으로 해주는거 쓰지 않기 - 물어보며 같이 만들기)
2. give up on editor-based agentic pairing in favor of asynchronous workflows

> **Why it matters:** 
> AI의 생산성 향상 vs 자신의 실력 향상 - 밸런스를 잡기 힘들다. 이 사이에서 어떻게 하는게 좋을까? 여기에 대한 가설 / 응답 / 컨센서스들이 만들어지는 중이다. 방향을 잡는 데 도움이 된다. 

### 5. Agentic Coding Recommendations
Claude Code 기반의 agentic coding 경험을 바탕으로 효율적이고 신뢰할 수 있는 개발 환경을 구축하기 위한 전략을 제시: 효율성과 안정성을 위해 도구 설계, 언어 선택, 로그 최적화, 병렬화, 단순한 코드 작성이 핵심

> **Why it matters:** 
> 에이전트가 코드를 생성·실행하는 새로운 패러다임에서, 효율적이고 견고한 개발 환경을 구축하는 방법론을 제시함으로써, 향후 LLM 기반 소프트웨어 개발의 실질적 기준점을 제시한다.

### 6. Field Notes From Shipping Real Code With Claude
코딩할 때 AI와의 협업을 강력히 추천하며, 협업할 때 도움이 될 팁에 관한 내용
함수별로 주석을 달아 AI와 협업:
• AIDEV-NOTE :  배경 설명, 접근 제약
• AIDEV-TODO : 해야할일 지시
• AIDEV-QUESTION: 불확실한 부분을 AI 한태 질문
반드시 사람이 해야하는것:
테스트 코드, API 계약, 버전 업데이트, 마이그레이션 (혹여나 오류가 발생시에 파급력이 너무 커지는 것)

> **Why it matters:** 
> AI와 협업하며 지켜야할 권장사항을 상당히 구체적으로 적어놓고, 실제로 유용할법한 내용.

## ⭐ 3점

### 1. Windsurf, 브라우저에서 바로 AI와 협업을 함께 할 수 있는 Windsurf Browser 베타 공개
windsurf Browser는 브라우저 내에서 사용자가 보고 있는 코드, 로그, 문서 내용을 그대로 Cascade에 전송할 수 있는 기능을 중심으로 설계된 새로운 웹 브라우저입니다. 웹을 탐색하다가 마주친 API 사용법, 콘솔 에러 메시지, UI 스니펫 등 개발과 관련된 거의 모든 정보를 선택만 하면, 별도의 복사 없이 바로 AI 어시스턴트에게 전달되어 상황에 맞는 코멘트나 코드 추천을 받을 수 있습니다. 이는 “지금 내가 보고 있는 것”을 AI가 직접 이해하게 만들어줍니다.

> **Why it matters:** 
> Why it matters:  기존의 AI 코드 어시스턴트는 주로 IDE 내부에서 작동하거나, 사용자가 컨텍스트를 직접 복사해 붙여넣어야 했습니다. 그 과정에서 많은 정보가 손실되거나, AI가 문맥을 제대로 파악하지 못해 반복적인 설명이 필요하곤 했습니다. Windsurf Browser는 이러한 과정을 생략합니다. 마우스로 내용을 선택하기만 하면 AI가 그 내용을 그대로 받아들이고, 필요한 코드를 제시하거나 오류의 원인을 분석해줍니다. 이는 특히 Stack Overflow, GitHub, 공식 문서 등 외부 리소스를 자주 참고하는 개발자에게 매우 유용합니다.
> 
> Windsurf Browser는 단순히 웹페이지를 띄우는 브라우저가 아닙니다. 마우스 드래그 또는 텍스트 선택을 통해 콘솔 에러, UI 코드, API 예제 등을 Cascade에 즉시 전달하고, 해당 컨텍스트를 이해한 AI가 대화를 이어가는 구조입니다. 이 구조는 특히 다음과 같은 상황에서 유용합니다:
> • 디버깅 중 콘솔 에러 메시지를 분석할 때
> • 복잡한 UI 코드나 CSS 구성을 설명받고자 할 때
> • 공식 문서나 블로그의 코드를 내 프로젝트에 맞게 적용하고자 할 때

### 2. V-JEPA 2: Open-Source Self-Supervised World Models for Understanding, Prediction, and Plannin
V-JEPA 2 is Meta AI’s upgraded vision-based world model that learns representations through self-supervised predictive tasks, without relying on reconstruction. Unlike traditional approaches, V-JEPA 2 focuses on predicting latent features of the future, allowing it to plan and generalize across diverse environments. It supports high-resolution inputs (up to 448×448), learns from videos with 100× fewer labels, and is now open-sourced for broader community use.

> **Why it matters:** 
> V-JEPA 2 represents a shift from pixel-level predictions to more abstract, efficient representation learning. Its ability to understand and predict future states without labeled data is crucial for building scalable and general-purpose AI agents, especially in robotics, autonomous systems, and embodied AI.

### 3. How I program with Agents
에이전트는 LLM 호출을 포함한 9줄의 for 루프로 정의되며, bash, patch, todo 등 프로그래머 친숙한 도구들을 활용해 인간 개입 없이 명령을 실행하고 결과를 확인할 수 있습니다.
저자는 GitHub App 인증 기능 구현에서 3-4번의 피드백만으로 일주일 분량의 작업을 하루 만에 완성했지만, 높은 시간/비용과 보안 위험, 코드 품질 문제 등의 한계가 있다고 언급했습니다.
2025년 LLM은 에이전트 구동에 최적화되어 프로그래밍 워크플로우와 업계 전반에 근본적 변화를 가져올 것이며, 프로그래머를 대체하는 것이 아닌 생산성 향상 도구로서 큰 가치가 있다고 결론지었습니다.

> **Why it matters:** 
> 에이전트를 이용한 프로그래밍 개발에 대한 인사이트를 제공합니다

### 4. Seven replies to the viral Apple reasoning paper – and why they fall short
애플이 6월 9일 공개한 “The Illusion of Thinking” 논문은 최신 대규모 추론 모델(LRM)이 문제 복잡도가 조금만 높아져도 ‘complete accuracy collapse(정확도 붕괴)’를 일으킨다고 지적했다. 기존 LLM보다 계산을 더 많이 투입해 단계별로 ‘생각하는’ LRM조차 하노이 탑·강 건너기 퍼즐처럼 유치원생도 푸는 논리 문제에서 크게 실패했으며, 이는 현행 ‘스케일링 가설’에 구조적 한계를 드러낸다는 주장이다.
이에 맞서 일부 연구자와 업계 인사들은 ▲사람도 복잡한 문제에서 종종 실패한다 ▲애플이 쓴 퍼즐·평가가 비현실적이다 ▲더 큰 모델·더 긴 컨텍스트·프롬프트 기법이면 해결된다 등 일곱 가지 반론을 제시했다. 그러나 가리 마커스는 자신의 칼럼 **“Seven replies to the viral Apple reasoning paper – and why they fall short”**에서 각각의 반론이 ‘사소한 트집(nit-picking)’부터 ‘교묘한 논점 흐리기’에 머무를 뿐, 논문의 핵심인 ‘복잡도 임계점에서의 붕괴’를 설명하지 못한다고 비판했다.
마커스는 “인간과 같은 실수를 한다”는 주장은 기계에게 인간을 뛰어넘는 일관성과 신뢰성을 요구하는 AI 개발 목표를 회피하는 논리일 뿐이며, “스케일링이 답”이라는 낙관론도 세일즈포스가 별도로 확인한 비슷한 붕괴 현상으로 반박된다고 강조했다. 결국 그는 현재의 순수 LLM·LRM 노선만으로는 AGI에 도달하기 어렵고, 상징적 추론·검증 가능한 하이브리드 접근이 필요하다는 결론을 내렸다.

> **Why it matters:** 
> 해당 내용은 “스케일만 키우면 AGI에 도달한다”는 지난 3년간의 주류 패러다임에 결정적 의문을 던짐. 애플·세일즈포스 같은 빅테크 내부에서조차 LLM 스케일링의 구조적 한계를 지적했다는 점. 마커스의 분석처럼 일곱 가지 반박이 설득력을 얻지 못한다면, 연구 자금과 인력은 대규모 파라미터 증설보다 하이브리드·상징 추론·검증가능성으로 이동할 가능성이 큼. 산업적으로는 ‘에이전트’ 자동화 열풍에 제동이 걸릴 수 있고, 규제 측면에서는 신뢰성·안전성 표준 요구가 강화될 것. 즉, 이번 해당 내용은 미래 LLM 로드맵, 투자 흐름, 정책 설계에 직접적인 영향을 주는 ‘트렌드 분기점’으로 작용될 것.

## ⭐ 2점

### 1. MemOS: A Memory-Centric Operating System for Evolving and Adaptive Large Language Models
요약 없음

> **Why it matters:** 
> 내용 없음

### 2. LLMs are cheap
요약 없음

> **Why it matters:** 
> 내용 없음

### 3. The first big AI disaster is yet to happen
요약 없음

> **Why it matters:** 
> 내용 없음

### 4. Andrew Ng: State of AI Agents | LangChain Interrupt
앤드류 응과의 fireside chat에서는 ai 에이전트의 현재 상태와 미래에 대한 통찰을 얻을 수 있습니다. 앤드류 응은 에이전트의 자율성 정도에 따라 agentic 시스템을 정의하고, 에이전트 구축에 필요한 기술과 도구에 대해 논의합니다. 특히, 평가(eval)의 중요성을 강조하며, 음성 스택(voice stack)과 mcp(modular component protocol)와 같은 기술에 주목합니다. 또한, ai 코딩 보조 도구를 활용한 코딩 방식과 모든 직군에서 코딩 능력을 갖추는 것의 중요성을 강조하며, AI가 코딩을 자동화할 것이라는 주장에 반박합니다. 궁극적으로, 이 대화는 ai 에이전트 기술의 발전 방향과 개발자들이 갖춰야 할 역량에 대한 균형 잡힌 시각을 제공합니다.

> **Why it matters:** 
> 이미 다 아는 이야기 

## ⭐ 1점

### 1. Nanonets-OCR-s: An Open-Source Image-to-Markdown Model with LaTeX, Tables, Signatures, checkboxes & Mor
OCR Api Nanonets-OCR-s 의 등장
OCR 이라고 소개하고 있지만  IDP(지능형 문서 처리) 에 가까운 형태
이미지에 자연어 뿐만아니라 표, 수식, 이미지, 서명 등도 분석하여 마크다운 형태로 제공함

> **Why it matters:** 
> Mcp와 연계하여 문서처리를 처리하기엔 유용하겠으나 아직 비용이 비쌈(종량제 기준 페이지당 0.3달러)  발전, 비용인하를 지켜볼 여지는 있음

### 2. The last six months in LLMs, illustrated by pelicans on bicycles
요약 없음

> **Why it matters:** 
> 내용 없음

### 3. Nvidia CEO slams Anthropic's chief over his claims of AI taking half of jobs and being unsafe — ‘Don’t do it in a dark room and tell me it’s safe’
요약 없음

> **Why it matters:** 
> 내용 없음
## 🔽 지난 주간 소식
<details>
<summary>📆 [2025/06/16 ~ 2025/06/22] 주간 소식</summary>

## 식
## ⭐ 4점

### 1. Anthropic의 멀티 에이전트 기반 연구 시스템: 아키텍처, 설계 전략, 성능 최적화
요약 없음

> **Why it matters:** 
> 내용 없음

### 2. 멀티모달 대형 언어모델이 집으로 가는 길을 안내할 수 있을까? 교통지도 기반 세밀한 시각적 추론 평가를 위한 벤치마크 연구 / Can MLLMs Guide Me Home? A Benchmark Study on Fine-Grained Visual Reasoning from Transit Maps
ReasonMap은 세밀한 시각적 추론 능력을 평가하기 위해 고해상도 교통 지도를 기반으로 만든 MLLM 벤치마크로, 기존 모델들의 시각적 추론 성능과 오픈소스/폐쇄형 모델 간 성능 차이를 드러낸다

> **Why it matters:** 
> 시각적 추론 능력은 멀티모달 AI의 핵심 과제이며, ReasonMap은 그동안 간과되었던 ‘정밀한 공간 추론’ 능력을 정량적으로 평가할 수 있는 첫 체계적 시도 중 하나로, MLLM의 한계와 발전 방향을 동시에 보여주기 때문이다.

### 3. Text-to-LoRA (T2L): A Hypernetwork that Generates Task-Specific LLM Adapters (LoRAs) based on a Text Description of the Task
	1.	Sakana AI의 Text-to-LoRA(T2L)는 자연어 설명만으로 LLM용 LoRA 어댑터를 자동 생성하는 기술입니다.
2.	별도의 훈련 없이 텍스트 입력만으로 다양한 작업에 맞는 어댑터를 즉시 만들 수 있습니다.
3.	기존 수동 방식과 비슷하거나 더 나은 성능을 보여, LLM 커스터마이징이 훨씬 쉬워졌습니다.

> **Why it matters:** 
> 기존에 많은 학습 리소스가 필요한 LoRA를 자연어 명령어로 zero-shot 업데이트를 할 수 있습니다

### 4. Why agents are bad pair programmers
LLM agents make bad pairs because they code faster than humans think.
1. throttle down from the semi-autonomous "Agent" mode to the turn-based "Edit" or "Ask" modes (자율적으로 해주는거 쓰지 않기 - 물어보며 같이 만들기)
2. give up on editor-based agentic pairing in favor of asynchronous workflows

> **Why it matters:** 
> AI의 생산성 향상 vs 자신의 실력 향상 - 밸런스를 잡기 힘들다. 이 사이에서 어떻게 하는게 좋을까? 여기에 대한 가설 / 응답 / 컨센서스들이 만들어지는 중이다. 방향을 잡는 데 도움이 된다. 

### 5. Agentic Coding Recommendations
Claude Code 기반의 agentic coding 경험을 바탕으로 효율적이고 신뢰할 수 있는 개발 환경을 구축하기 위한 전략을 제시: 효율성과 안정성을 위해 도구 설계, 언어 선택, 로그 최적화, 병렬화, 단순한 코드 작성이 핵심

> **Why it matters:** 
> 에이전트가 코드를 생성·실행하는 새로운 패러다임에서, 효율적이고 견고한 개발 환경을 구축하는 방법론을 제시함으로써, 향후 LLM 기반 소프트웨어 개발의 실질적 기준점을 제시한다.

### 6. Field Notes From Shipping Real Code With Claude
코딩할 때 AI와의 협업을 강력히 추천하며, 협업할 때 도움이 될 팁에 관한 내용
함수별로 주석을 달아 AI와 협업:
• AIDEV-NOTE :  배경 설명, 접근 제약
• AIDEV-TODO : 해야할일 지시
• AIDEV-QUESTION: 불확실한 부분을 AI 한태 질문
반드시 사람이 해야하는것:
테스트 코드, API 계약, 버전 업데이트, 마이그레이션 (혹여나 오류가 발생시에 파급력이 너무 커지는 것)

> **Why it matters:** 
> AI와 협업하며 지켜야할 권장사항을 상당히 구체적으로 적어놓고, 실제로 유용할법한 내용.

## ⭐ 3점

### 1. Windsurf, 브라우저에서 바로 AI와 협업을 함께 할 수 있는 Windsurf Browser 베타 공개
windsurf Browser는 브라우저 내에서 사용자가 보고 있는 코드, 로그, 문서 내용을 그대로 Cascade에 전송할 수 있는 기능을 중심으로 설계된 새로운 웹 브라우저입니다. 웹을 탐색하다가 마주친 API 사용법, 콘솔 에러 메시지, UI 스니펫 등 개발과 관련된 거의 모든 정보를 선택만 하면, 별도의 복사 없이 바로 AI 어시스턴트에게 전달되어 상황에 맞는 코멘트나 코드 추천을 받을 수 있습니다. 이는 “지금 내가 보고 있는 것”을 AI가 직접 이해하게 만들어줍니다.

> **Why it matters:** 
> Why it matters:  기존의 AI 코드 어시스턴트는 주로 IDE 내부에서 작동하거나, 사용자가 컨텍스트를 직접 복사해 붙여넣어야 했습니다. 그 과정에서 많은 정보가 손실되거나, AI가 문맥을 제대로 파악하지 못해 반복적인 설명이 필요하곤 했습니다. Windsurf Browser는 이러한 과정을 생략합니다. 마우스로 내용을 선택하기만 하면 AI가 그 내용을 그대로 받아들이고, 필요한 코드를 제시하거나 오류의 원인을 분석해줍니다. 이는 특히 Stack Overflow, GitHub, 공식 문서 등 외부 리소스를 자주 참고하는 개발자에게 매우 유용합니다.
> 
> Windsurf Browser는 단순히 웹페이지를 띄우는 브라우저가 아닙니다. 마우스 드래그 또는 텍스트 선택을 통해 콘솔 에러, UI 코드, API 예제 등을 Cascade에 즉시 전달하고, 해당 컨텍스트를 이해한 AI가 대화를 이어가는 구조입니다. 이 구조는 특히 다음과 같은 상황에서 유용합니다:
> • 디버깅 중 콘솔 에러 메시지를 분석할 때
> • 복잡한 UI 코드나 CSS 구성을 설명받고자 할 때
> • 공식 문서나 블로그의 코드를 내 프로젝트에 맞게 적용하고자 할 때

### 2. V-JEPA 2: Open-Source Self-Supervised World Models for Understanding, Prediction, and Plannin
V-JEPA 2 is Meta AI’s upgraded vision-based world model that learns representations through self-supervised predictive tasks, without relying on reconstruction. Unlike traditional approaches, V-JEPA 2 focuses on predicting latent features of the future, allowing it to plan and generalize across diverse environments. It supports high-resolution inputs (up to 448×448), learns from videos with 100× fewer labels, and is now open-sourced for broader community use.

> **Why it matters:** 
> V-JEPA 2 represents a shift from pixel-level predictions to more abstract, efficient representation learning. Its ability to understand and predict future states without labeled data is crucial for building scalable and general-purpose AI agents, especially in robotics, autonomous systems, and embodied AI.

### 3. How I program with Agents
에이전트는 LLM 호출을 포함한 9줄의 for 루프로 정의되며, bash, patch, todo 등 프로그래머 친숙한 도구들을 활용해 인간 개입 없이 명령을 실행하고 결과를 확인할 수 있습니다.
저자는 GitHub App 인증 기능 구현에서 3-4번의 피드백만으로 일주일 분량의 작업을 하루 만에 완성했지만, 높은 시간/비용과 보안 위험, 코드 품질 문제 등의 한계가 있다고 언급했습니다.
2025년 LLM은 에이전트 구동에 최적화되어 프로그래밍 워크플로우와 업계 전반에 근본적 변화를 가져올 것이며, 프로그래머를 대체하는 것이 아닌 생산성 향상 도구로서 큰 가치가 있다고 결론지었습니다.

> **Why it matters:** 
> 에이전트를 이용한 프로그래밍 개발에 대한 인사이트를 제공합니다

### 4. Seven replies to the viral Apple reasoning paper – and why they fall short
애플이 6월 9일 공개한 “The Illusion of Thinking” 논문은 최신 대규모 추론 모델(LRM)이 문제 복잡도가 조금만 높아져도 ‘complete accuracy collapse(정확도 붕괴)’를 일으킨다고 지적했다. 기존 LLM보다 계산을 더 많이 투입해 단계별로 ‘생각하는’ LRM조차 하노이 탑·강 건너기 퍼즐처럼 유치원생도 푸는 논리 문제에서 크게 실패했으며, 이는 현행 ‘스케일링 가설’에 구조적 한계를 드러낸다는 주장이다.
이에 맞서 일부 연구자와 업계 인사들은 ▲사람도 복잡한 문제에서 종종 실패한다 ▲애플이 쓴 퍼즐·평가가 비현실적이다 ▲더 큰 모델·더 긴 컨텍스트·프롬프트 기법이면 해결된다 등 일곱 가지 반론을 제시했다. 그러나 가리 마커스는 자신의 칼럼 **“Seven replies to the viral Apple reasoning paper – and why they fall short”**에서 각각의 반론이 ‘사소한 트집(nit-picking)’부터 ‘교묘한 논점 흐리기’에 머무를 뿐, 논문의 핵심인 ‘복잡도 임계점에서의 붕괴’를 설명하지 못한다고 비판했다.
마커스는 “인간과 같은 실수를 한다”는 주장은 기계에게 인간을 뛰어넘는 일관성과 신뢰성을 요구하는 AI 개발 목표를 회피하는 논리일 뿐이며, “스케일링이 답”이라는 낙관론도 세일즈포스가 별도로 확인한 비슷한 붕괴 현상으로 반박된다고 강조했다. 결국 그는 현재의 순수 LLM·LRM 노선만으로는 AGI에 도달하기 어렵고, 상징적 추론·검증 가능한 하이브리드 접근이 필요하다는 결론을 내렸다.

> **Why it matters:** 
> 해당 내용은 “스케일만 키우면 AGI에 도달한다”는 지난 3년간의 주류 패러다임에 결정적 의문을 던짐. 애플·세일즈포스 같은 빅테크 내부에서조차 LLM 스케일링의 구조적 한계를 지적했다는 점. 마커스의 분석처럼 일곱 가지 반박이 설득력을 얻지 못한다면, 연구 자금과 인력은 대규모 파라미터 증설보다 하이브리드·상징 추론·검증가능성으로 이동할 가능성이 큼. 산업적으로는 ‘에이전트’ 자동화 열풍에 제동이 걸릴 수 있고, 규제 측면에서는 신뢰성·안전성 표준 요구가 강화될 것. 즉, 이번 해당 내용은 미래 LLM 로드맵, 투자 흐름, 정책 설계에 직접적인 영향을 주는 ‘트렌드 분기점’으로 작용될 것.

## ⭐ 2점

### 1. MemOS: A Memory-Centric Operating System for Evolving and Adaptive Large Language Models
요약 없음

> **Why it matters:** 
> 내용 없음

### 2. LLMs are cheap
요약 없음

> **Why it matters:** 
> 내용 없음

### 3. The first big AI disaster is yet to happen
요약 없음

> **Why it matters:** 
> 내용 없음

### 4. Andrew Ng: State of AI Agents | LangChain Interrupt
앤드류 응과의 fireside chat에서는 ai 에이전트의 현재 상태와 미래에 대한 통찰을 얻을 수 있습니다. 앤드류 응은 에이전트의 자율성 정도에 따라 agentic 시스템을 정의하고, 에이전트 구축에 필요한 기술과 도구에 대해 논의합니다. 특히, 평가(eval)의 중요성을 강조하며, 음성 스택(voice stack)과 mcp(modular component protocol)와 같은 기술에 주목합니다. 또한, ai 코딩 보조 도구를 활용한 코딩 방식과 모든 직군에서 코딩 능력을 갖추는 것의 중요성을 강조하며, AI가 코딩을 자동화할 것이라는 주장에 반박합니다. 궁극적으로, 이 대화는 ai 에이전트 기술의 발전 방향과 개발자들이 갖춰야 할 역량에 대한 균형 잡힌 시각을 제공합니다.

> **Why it matters:** 
> 이미 다 아는 이야기 

## ⭐ 1점

### 1. Nanonets-OCR-s: An Open-Source Image-to-Markdown Model with LaTeX, Tables, Signatures, checkboxes & Mor
OCR Api Nanonets-OCR-s 의 등장
OCR 이라고 소개하고 있지만  IDP(지능형 문서 처리) 에 가까운 형태
이미지에 자연어 뿐만아니라 표, 수식, 이미지, 서명 등도 분석하여 마크다운 형태로 제공함

> **Why it matters:** 
> Mcp와 연계하여 문서처리를 처리하기엔 유용하겠으나 아직 비용이 비쌈(종량제 기준 페이지당 0.3달러)  발전, 비용인하를 지켜볼 여지는 있음

### 2. The last six months in LLMs, illustrated by pelicans on bicycles
요약 없음

> **Why it matters:** 
> 내용 없음

### 3. Nvidia CEO slams Anthropic's chief over his claims of AI taking half of jobs and being unsafe — ‘Don’t do it in a dark room and tell me it’s safe’
요약 없음

> **Why it matters:** 
> 내용 없음

</details>
</details>