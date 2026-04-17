<div align="center">

# PCG_BuildingSample

Unreal Engine 5의 **PCG(Procedural Content Generation)** 프레임워크를 활용해 빌딩을 절차적으로 배치하는 샘플 프로젝트입니다.

![Unreal Engine](https://img.shields.io/badge/Unreal_Engine-5.7-0E1128?style=for-the-badge&logo=unrealengine&logoColor=white)
![PCG](https://img.shields.io/badge/Plugin-PCG-5A9FD4?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)
![Platform](https://img.shields.io/badge/Platform-Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white)

</div>

## 목차

- [개요](#개요)
- [주요 기능](#주요-기능)
- [환경](#환경)
- [주요 에셋](#주요-에셋)
- [사용 방법](#사용-방법)
- [프로젝트 구조](#프로젝트-구조)
- [라이선스](#라이선스)

## 개요

영역을 지정하면 PCG 그래프가 규칙에 따라 건물을 자동으로 배치해 도시/거리 환경을 빠르게 구성할 수 있도록 구현한 예시입니다.

## 주요 기능

- 🏙️ **절차적 빌딩 배치** — PCG 그래프 기반의 자동 배치 시스템
- 🧩 **모듈형 건물 에셋** — ResidentialBuildingsSet 활용
- 🌊 **환경 요소 포함** — 강(River) 블루프린트, 도로/지형 머티리얼
- 🎮 **즉시 실행 가능** — 샘플 레벨(Lvl_PCGSample) 제공

## 환경

| 항목 | 버전/설명 |
| --- | --- |
| Unreal Engine | 5.7 |
| 필수 플러그인 | PCG, ModelingToolsEditorMode, GameplayStateTree |

## 주요 에셋

| 경로 | 설명 |
| --- | --- |
| `Content/PCG_Building/PCG/PCG_Building` | 빌딩 배치용 PCG 그래프 |
| `Content/PCG_Building/Blueprints/PCG_BuildingGenerator` | PCG를 사용하는 제너레이터 블루프린트 |
| `Content/PCG_Building/Blueprints/BP_River` | 강/수로 블루프린트 |
| `Content/PCG_Building/Level/Lvl_PCGSample` | 샘플 레벨 |
| `Content/ResidentialBuildingsSet` | 배치에 사용되는 건물 모듈 에셋 |

## 사용 방법

1. `PCG_BuildingSample.uproject`를 UE 5.7에서 엽니다.
2. `Content/PCG_Building/Level/Lvl_PCGSample`을 로드합니다.
3. 레벨 내 `PCG_BuildingGenerator` 액터를 선택해 스플라인/영역을 수정하면 빌딩이 자동 재배치됩니다.
4. 필요에 따라 `PCG_Building` 그래프를 열어 규칙(크기, 간격, 건물 종류 등)을 커스터마이즈합니다.

## 프로젝트 구조

```
PCG_BuildingSample/
├── Config/                          # 프로젝트 설정 파일
├── Content/
│   ├── PCG_Building/
│   │   ├── Blueprints/              # BP_River, PCG_BuildingGenerator
│   │   ├── Level/                   # Lvl_PCGSample
│   │   ├── Materials/               # 지형/도로/물 머티리얼
│   │   ├── PCG/                     # PCG_Building 그래프
│   │   └── Textures/
│   └── ResidentialBuildingsSet/     # 건물 모듈 에셋
└── PCG_BuildingSample.uproject
```

## 라이선스

[MIT License](LICENSE) © 2026 DrunkenPoy
