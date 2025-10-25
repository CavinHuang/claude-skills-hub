# Claude Skills Hub

<div align="center">

![Claude Skills Hub](https://img.shields.io/badge/Claude-Skills%20Hub-blue?style=for-the-badge)
![Platform](https://img.shields.io/badge/Platform-Web-green?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)
![Version](https://img.shields.io/badge/Version-0.1.0-orange?style=for-the-badge)

**🤖 Claude Skills Hub - Claude 스킬 발견 및 다운로드**

[![Live Demo](https://img.shields.io/badge/🌐-Live%20Demo-informational)](https://claudeskill.site)
[![Documentation](https://img.shields.io/badge/📚-Documentation-blue)](docs/)
[![Get Started](https://img.shields.io/badge/🚀-Get%20Started-success)](#시작하기)

</div>

## 언어 / Language

- [English](README.md)
- [中文简体](README_ZH.md)
- [日本語](README_JA.md)
- **한국어** (현재)
- [Français](README_FR.md)
- [Español](README_ES.md)

## 📋 프로젝트 개요

Claude Skills Hub는 Claude 사용자에게 실용적인 스킬 템플릿과 도구를 제공하는 오픈소스 AI 스킬 공유 플랫폼입니다. 이 프로젝트는 다양한 Claude 스킬의 수집, 정리, 공유에 중점을 두어 사용자의 작업 효율성 향상을 지원합니다.

### 🎯 프로젝트 목표

- **📝 스킬 수집**: 실용적인 Claude 스킬 템플릿 수집 및 정리
- **🔧 도구 개발**: 코드 생성, 문서 작성 등 실용적인 도구 제공
- **📚 지식 공유**: 스킬 공유 및 학습을 위한 커뮤니티 플랫폼 구축
- **🚀 효율성 향상**: 사용자가 적절한 AI 스킬을 빠르게 찾고 사용할 수 있도록 지원

## ✨ 현재 기능

### 📖 스킬 문서
- **스킬 템플릿**: 표준화된 스킬 설명 형식
- **사용 가이드**: 상세한 스킬 사용 설명 및 예제
- **카테고리 관리**: 기능 영역별 스킬 분류

### 🛠️ 기본 도구
- **문서 생성**: 기본 문서 템플릿 및 형식
- **코드 예제**: 일반적인 코드 스니펫 및 템플릿

### 🌍 커뮤니티 구축
- **오픈 기여**: 커뮤니티 개발자의 스킬 및 개선 기여 환영
- **문서 표준**: 통일된 스킬 문서 규범 확립

## 📊 프로젝트 현황

<div align="center">

| 지표 | 현재 상태 | 설명 |
|------|-----------|------|
| 📋 스킬 수 | 3개 예제 | 비즈니스 문서, UI 컴포넌트, 코드 생성기 |
| 📂 스킬 카테고리 | 8개 카테고리 | 개발, 디자인, 비즈니스 등 |
| 📚 문서 완성도 | 기본 버전 | 사용자 가이드 및 개발자 문서 |
| 🚀 프로젝트 단계 | 초기 개발 | 기여 및 피드백 환영 |

</div>

## 🎯 스킬 카테고리

이 프로젝트는 다음 카테고리로 AI 스킬을 정리하며, 현재 예제 템플릿을 제공합니다:

### 🔧 개발 (Development)
- **코드 생성기**: 다양한 프로그래밍 언어 코드 템플릿 생성
- **API 문서 생성**: API 인터페이스 문서 작성
- **테스트 코드**: 단위 테스트 및 테스트 케이스 생성

### 🎨 디자인 (Design)  
- **UI 컴포넌트 생성**: React/Vue/Angular 컴포넌트 템플릿
- **디자인 문서**: 디자인 사양 및 설명 문서

### 💼 비즈니스 (Business)
- **비즈니스 문서**: 사업 계획서, 제안서 등 문서 템플릿
- **분석 보고서**: 데이터 분석 및 보고서 형식

### 📝 콘텐츠 (Content)
- **글쓰기**: 블로그 및 기술 기사 템플릿
- **문서 작성**: 기술 문서 및 설명서

### 🎓 교육 (Education)
- **교육 자료**: 과정 설계 및 교육 자료
- **학습 가이드**: 학습 경로 및 튜토리얼 템플릿

*참고: 기타 카테고리(분석, 연구, 엔터테인먼트)는 계획 중입니다. 기여를 환영합니다.*

## 🚀 시작하기

### 스킬 사용

1. **스킬 탐색**
   - [claudeskill.site](https://claudeskill.site)를 방문하여 사용 가능한 스킬 확인
   - `skills/` 디렉토리에서 스킬 문서 확인

2. **스킬 템플릿 사용**
   - 해당 스킬의 SKILL.md 내용 복사
   - 설명에 따라 Claude에서 스킬 사용

### 개발 및 기여

1. **프로젝트 클론**
   ```bash
   git clone https://github.com/CavinHuang/claude-skills-hub.git
   cd claude-skills-hub
   ```

2. **새 스킬 추가**
   - `skills/` 디렉토리에 새 스킬 폴더 생성
   - 기존 형식에 따라 SKILL.md 문서 작성

3. **기여 제출**
   ```bash
   git add .
   git commit -m "feat: add new skill"
   git push origin feature/new-skill
   ```

## 🛠️ 기술 아키텍처

이 프로젝트는 간단한 정적 파일 구조를 사용합니다:

- **프론트엔드**: Next.js 14 + TypeScript
- **스타일링**: Tailwind CSS
- **배포**: Vercel
- **문서**: Markdown 형식

## 📚 문서 리소스

- **[사용자 가이드](docs/user-guide.md)**: 사용 설명 및 튜토리얼
- **[개발자 문서](docs/developer-guide.md)**: 기술 문서 및 개발 가이드
- **[기여 가이드](CONTRIBUTING.md)**: 프로젝트 기여 참여 방법

## 🤝 기여 가이드

모든 형태의 기여를 환영합니다!

### 기여 방법
- 🎯 새로운 스킬 템플릿 추가
- 📝 기존 문서 개선  
- 🐛 문제 수정
- 💡 기능 제안

### 기여 프로세스
1. 프로젝트 저장소 포크
2. 기능 브랜치 생성
3. 변경 사항 제출
4. 풀 리퀘스트 생성

자세한 기여 가이드라인은 [CONTRIBUTING.md](CONTRIBUTING.md)를 참조하세요.

## 📄 라이선스

이 프로젝트는 [MIT 라이선스](LICENSE) 하에 라이선스됩니다 - 자유롭게 사용, 수정, 배포하세요.

## 🙏 감사의 말

Claude Skills Hub에 기여해주신 모든 개발자분들께 감사드립니다!

### 기여자
- [@CavinHuang](https://github.com/CavinHuang) - 프로젝트 생성자

### 특별 감사
- Anthropic Claude 팀 - AI 기술 지원 제공
- 오픈소스 커뮤니티 - 영감과 기술 지원 제공

## 📞 연락처

- **🌐 웹사이트**: [https://claudeskill.site](https://claudeskill.site)
- **💬 토론**: [GitHub Discussions](https://github.com/CavinHuang/claude-skills-hub/discussions)
- **🐛 이슈**: [GitHub Issues](https://github.com/CavinHuang/claude-skills-hub/issues)

---

<div align="center">

**⭐ 이 프로젝트가 도움이 되셨다면 Star를 눌러주세요!**

</div>