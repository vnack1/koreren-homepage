## **Brand Homepage (React + Tailwind CSS + Supabase + Node/Express)**

**브랜드 스토리/ 상품 상세페이지/ 파트너십/ 제휴 문의**를 위한 브랜드 홈페이지. 프론트엔드(React/Tailwind)와 백엔드(Express/Supabase)를 분리하여, **배포 민첩성**과 **운영 편의성**을 동시에 확보

### **배포 주소**

- **URL**: [https://koreren.co.kr](https://koreren.co.kr/) //현재 다른 외주개발사가 관리중

### **역할**

- 프론트엔드 UI/UX, Tailwind 기반 디자인 시스템, GSAP/Lenis 애니메이션 구현
- 백엔드 API/DB 연동(Supabase) 및 이미지/메일 파이프라인 구현
- Vercel/Render/Supabase 연계 배포 및 환경 변수 스키마화

### **기술 스택**

- **Frontend**: React, Vite, Tailwind, GSAP(ScrollTrigger), Lenis, React Router, TipTap
- **Backend**: Node.js(ESM), Express 5, Supabase JS, Sharp, Formidable, Nodemailer, Gmail API, KakaoMap API
- **Deploy**: Vercel(프론트), Render(서버), Supabase(DB/Storage)

### **아키텍처**

- **프론트엔드**: components/Header/Footer/Canonical/ScrollToTop, pages/Home/About/Partners/Contact/Notices
- **백엔드**: config, utils, controllers, services, models, routes, validates
- **데이터 계층**: Supabase 서비스롤 키 서버에서만 사용 → 보안 강화

### **핵심 기능**

- **문의(Contact)**: Gmail API + Nodemailer 연동, 제품 및 일반 문의 처리
- **파트너(Partners)**: Supabase 데이터 기반 + KakaoMap API로 위치 표시
- **공지(Notices)**: TipTap 기반 리치 텍스트 작성, Supabase 테이블 관리
- **SEO 최적화**: Canonical 태그, Scroll 성능 최적화(GSAP+Lenis)

### **차별점(강점)**

- 클라이언트/서버 **분리 배포(Vercel+Render)** → 각 레이어 릴리즈 민첩성
- Supabase 기반 데이터/스토리지/인증 통합
