# Southmw's GitHub Pages

이 저장소는 **Blazor WebAssembly** 웹 애플리케이션을 GitHub Pages에 배포하는 프로젝트입니다.

## 🚀 프로젝트 정보

- **프레임워크**: .NET 8.0 Blazor WebAssembly
- **배포 플랫폼**: GitHub Pages
- **패키지**: Bluehill.Blazor.GHPages, PublishSPAforGitHubPages.Build
- **서비스 워커**: 지원 (PWA 기능)

## 📁 프로젝트 구조

```
GithubIO/
├── Pages/           # Blazor 페이지 컴포넌트
│   ├── Home.razor   # 홈페이지
│   ├── Counter.razor # 카운터 페이지
│   └── Weather.razor # 날씨 페이지
├── Layout/          # 레이아웃 컴포넌트
├── wwwroot/         # 정적 파일
└── Program.cs       # 애플리케이션 진입점
```

## 🛠️ 로컬 개발

### 필요 조건
- .NET 8.0 SDK 이상
- Git

### 실행 방법
```bash
cd GithubIO
dotnet restore
dotnet run
```

브라우저에서 `https://localhost:5001`으로 접속하여 애플리케이션을 확인할 수 있습니다.

## 🌐 배포

이 프로젝트는 GitHub Actions를 통해 자동으로 GitHub Pages에 배포됩니다.

### 배포 과정
1. 코드를 `main` 브랜치에 푸시
2. GitHub Actions가 자동으로 빌드 및 배포 실행
3. 배포된 사이트는 `https://southmw.github.io`에서 확인 가능

### 수동 배포 (필요시)
```bash
cd GithubIO
dotnet publish -c Release
# 배포 파일은 bin/Release/net8.0/publish/ 폴더에 생성됩니다
```

## 🔧 기술 스택

- **Frontend**: Blazor WebAssembly
- **Styling**: Bootstrap 5
- **PWA**: Service Worker 지원
- **Deployment**: GitHub Pages + GitHub Actions

## 📝 라이선스

이 프로젝트는 MIT 라이선스 하에 배포됩니다.

## 📞 연락처

프로젝트에 대한 문의사항이 있으시면 [Issues](https://github.com/southmw/southmw.github.io/issues)를 통해 연락해 주세요.
