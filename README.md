# PCG_BuildingSample

Unreal Engine 5의 **PCG(Procedural Content Generation)** 프레임워크를 활용해 빌딩을 절차적으로 배치하는 샘플 프로젝트입니다.

## 개요

영역을 지정하면 PCG 그래프가 규칙에 따라 건물을 자동으로 배치해 도시/거리 환경을 빠르게 구성할 수 있도록 구현한 예시입니다.

## 환경

- **Unreal Engine**: 5.7
- **필수 플러그인**: PCG, ModelingToolsEditorMode, GameplayStateTree

## 주요 에셋

- `Content/PCG_Building/PCG/PCG_Building` — 빌딩 배치용 PCG 그래프
- `Content/PCG_Building/Blueprints/PCG_BuildingGenerator` — PCG를 사용하는 제너레이터 블루프린트
- `Content/PCG_Building/Blueprints/BP_River` — 강/수로 블루프린트
- `Content/PCG_Building/Level/Lvl_PCGSample` — 샘플 레벨
- `Content/ResidentialBuildingsSet` — 배치에 사용되는 건물 모듈 에셋

## 사용 방법

1. `PCG_BuildingSample.uproject`를 UE 5.7에서 엽니다.
2. `Content/PCG_Building/Level/Lvl_PCGSample`을 로드합니다.
3. 레벨 내 `PCG_BuildingGenerator` 액터를 선택해 스플라인/영역을 수정하면 빌딩이 자동 재배치됩니다.
4. 필요에 따라 `PCG_Building` 그래프를 열어 규칙(크기, 간격, 건물 종류 등)을 커스터마이즈합니다.

## 라이선스

[MIT License](LICENSE) © 2026 DrunkenPoy
