# 연습: 프롬프트 플러그인 만들기

이 연습에서는 다음 내용을 알아봅니다.

- 좋은 프롬프트를 작성하는 방법
- Copilot Studio에서 프롬프트를 만드는 방법
- 프롬프트 작성기에서 프롬프트를 테스트하는 방법
- Microsoft 365 Copilot에서 프롬프트 플러그인을 사용하는 방법

## 좋은 프롬프트를 작성하는 방법

이 모듈의 앞부분에서 이미 프롬프트 엔지니어링의 몇 가지 기본 사항을 알아보았습니다. 프롬프트 엔지니어링에 대해 자세히 알아볼 수 있는 유용한 리소스는 AI Builder 팀의 프롬프트 엔지니어링 가이드를 읽는 것입니다. 프롬프트 엔지니어링 가이드는 [여기](https://aka.ms/learn-ai-builder-prompting-guide)에서 찾을 수 있습니다.

## 좋은 프롬프트의 요소

AI Builder 팀의 프롬프트 엔지니어링 가이드에는 프롬프트에 포함시켜야 할 훌륭한 요소가 모여 있습니다.

보이는 바와 같이 다음과 같은 요소가 있습니다.

- **작업**: GPT(생성형 사전 학습 트랜스포머) 모델에게 수행할 작업을 알리는 **명령**
- **컨텍스트**: 작업 대상 **데이터**를 설명하고, 입력 **변수**가 있는 경우 함께 설명
- **기대치**: GPT에게 응답에 대한 **목표** 및 **기대치** 전달
- **출력**: GPT가 **출력**의 형식을 사용자가 원하는 방식으로 지정하도록 지원

![AI Builder 프롬프트 엔지니어링 가이드의 프롬프트 재료 페이지 스크린샷. 프롬프트 재료로 작업, 컨텍스트, 기대치, 출력이 강조 표시되어 있습니다.](../Media/4-prompt-engineering-guide.png)

## 작업 1: 프롬프트 디자인

이 작업에서는 경력 마일스톤을 기반으로 전문성 개발 계획을 세우는 데 도움이 되는 프롬프트를 디자인합니다.

> [!IMPORTANT]
> 프롬프트를 만들 때 처음부터 시작할 필요는 없습니다. 좋은 프롬프트를 작성하는 방법을 알아 두면 큰 도움이 되지만, 바로 목표에 반쯤 데려다 주는 리소스를 가지고 시작하는 것도 유용할 수 있습니다.
> [Microsoft 채택 샘플 솔루션 갤러리](https://aka.ms/power-prompts)에 바로 사용할 수 있는 프롬프트 샘플이 있습니다. 이 연습에서는 [Professional Development Plan 프롬프트 샘플](https://adoption.microsoft.com/sample-solution-gallery/sample/pnp-powerplatform-prompts-professional-development/)을 사용합니다.

프롬프트 재료를 모두 추가해 보겠습니다.

- **작업** - 전문성 개발 계획을 디자인합니다.
- **컨텍스트** - 다음 경력 [milestones] 달성을 목표로 하는 사람을 위한 것입니다.
- **기대치** - 계획에는 목표와 하위 목표, 리소스, 도구, 활동 타임라인이 포함되어야 합니다.
- **출력** - 계획을 간결하고 실행 가능한 형식으로 만들고 주니어 수준 직원에게 적합하도록 명확하고 따르기 쉬운 방식으로 정보를 제공합니다.

조합하면 다음과 같은 프롬프트가 됩니다.

*다음 경력 [마일스톤] 달성을 목표로 하는 사람을 위한 전문성 개발 계획을 설계해 줄래? 이 계획에는 목표와 하위 목표, 리소스, 도구, 활동에 대한 타임라인이 포함되어 있어야 해. 계획의 형식은 간결하고 실행 가능하게 만들고, 주니어 수준 직원에게 적합하도록 명확하고 따르기 쉬운 방식으로 정보를 제공해 줘.*

## 작업 2: Copilot Studio에서 프롬프트 작업 만들기

프롬프트 작성을 마쳤으므로 이제 Copilot Studio에 입력해야 합니다.

1. 웹 브라우저에서 [Copilot Studio](https://copilotstudio.microsoft.com)로 이동하고, 메시지가 표시되면 회사 또는 학교 계정으로 로그인합니다.  **건너뛰기**를 선택하여 환영 메시지를 건너뜁니다.

    **참고:** Copilot Studio를 처음 열면 첫 번째 Copilot을 만들기 위한 채팅 인터페이스가 표시될 수 있습니다. 이 경우 오른쪽 위 **...** 메뉴(**만들기** 버튼 옆)를 선택하고 **Copilot 만들기 취소**를 선택한 뒤 **나가기**를 선택하여 채팅 인터페이스를 나가서 Copilot Studio 홈페이지를 봅니다.
1. 왼쪽 탐색 영역에서 **라이브러리**를 선택합니다. 여기서는 기존 작업 및 커넥터 목록을 보고 새로 만들 수 있습니다.
1. 맨 위에 있는 **항목 추가**를 선택합니다.  메뉴에 Microsoft 365용 Copilot 확장 옵션 2가지가 나열됩니다.
:::image type="content" source="../Media/extend copilot options.png" alt-text="창에 Copilot 만들기 또는 작업 만들기라는 Copilot 확장 옵션 2가지가 나열됩니다.":::
1. **새 작업**를 선택합니다.
1. *새 작업* 화면에서 **프롬프트**를 선택합니다. 그러면 AI Builder 프롬프트 작성기가 열립니다.
1. **작업 세부 정보** 페이지에서 **작업 이름**으로 "Professional Development Plan"을 입력합니다.
1. 다음 **설명**을 입력합니다. "Creates an actionable professional development plan based on desired career milestones."
1. **다음**을 선택합니다.
1. **프롬프트 작업 추가** 페이지의 **프롬프트** 섹션에 다음 내용을 입력합니다. “다음 경력 [마일스톤] 달성을 목표로 하는 사람을 위한 전문성 개발 계획을 설계해 줄래? 이 계획에는 목표와 하위 목표, 리소스, 도구, 활동에 대한 타임라인이 포함되어 있어야 해. 계획의 형식은 간결하고 실행 가능하게 만들고, 주니어 수준 직원에게 적합하도록 명확하고 따르기 쉬운 방식으로 정보를 제공해 줘.” 이 내용을 **프롬프트**로 입력합니다.

    > [!NOTE]
    > 위쪽에 프롬프트에는 동적 값이 하나 이상 있어야 한다는 내용의 정보 표시줄이 있다는 것을 확인합니다.

1. 오른쪽 사이드바의 **프롬프트 설정**에서 **입력** 섹션을 엽니다.
1. **입력 추가** 버튼을 선택하여 입력을 추가합니다.
1. 입력 이름으로 `milestones`을(를) 입력합니다.
1. 샘플 데이터로 다음 텍스트를 추가합니다.

      ```text
      * Become medior in 3 years
      * Have 3 top reviews in a row
      * Become a manager in 10 years
      ```

1. 커서로 프롬프트 섹션의 **[milestones]** 를 선택합니다.
1. **삽입**을 선택합니다.
1. **milestones**를 선택합니다.

      그러면 **[milestones]** 값이 동적 값으로 변합니다.

1. 다음으로 프롬프트를 테스트할 준비가 되었습니다.

## 작업 3: 프롬프트 작성기에서 프롬프트 테스트

1. 프롬프트 섹션 아래의 **프롬프트 테스트**를 선택합니다. 이렇게 하면 이전에 추가한 샘플 데이터로 프롬프트가 테스트됩니다.

    > [!NOTE]
    > 그러면 프롬프트가 AI 모델로 보내지고 AI 응답 섹션에 응답이 표시됩니다. 이를 통해 LLM이 응답하는 방식을 보고 마음에 드는 결과가 나올지 확인할 수 있습니다.

1. AI 응답이 마음에 들면 **사용자 지정 프롬프트 저장**을 선택하여 프롬프트를 저장합니다.

    다음 창에서는 플러그인 설명 및 입력 설명을 검토할 수 있습니다.

1. **작업 매개 변수 선택** 페이지에서 **milestones**의 입력 설명을 다음과 같이 변경합니다.

      ```text
      The career milestones that the user wants to achieve
      ```

1. **다음**을 선택합니다.

1. **게시**를 선택하여 작업을 Microsoft 365 Copilot에 게시합니다.  1분 정도 걸릴 수 있습니다.

## 작업 4: Microsoft 365 Copilot에서 프롬프트 플러그인 사용

프롬프트 작업을 만들고 테스트했으므로 다음 작업을 계속 진행하여 Microsoft 365 Copilot에서 만든 프롬프트 작업에 액세스합니다.  플러그인이 Microsoft 365 Copilot에 표시되는 데 5분 이상 걸릴 수 있습니다.

1. [Microsoft Teams](https://teams.microsoft.com)를 엽니다.
1. 왼쪽 탐색 영역에서 **Copilot** 버튼을 선택합니다.
1. 화면 아래쪽의 **Copilot 응답 관리** 아이콘을 선택합니다(Copilot에게 메시지를 보낼 수 있는 위치 옆).
1. 나타난 플라이아웃 메뉴에서 **Copilot Studio**를 찾고, 사용하도록 설정했는지 확인합니다.  
1. Copilot Studio에서 작업 목록을 확장하기 위해 **캐럿 아이콘**을 선택합니다.

    > [!NOTE]
    > Copilot Studio가 보이지 않을 수도 있습니다. 이 경우 두 가지 이유가 있을 수 있습니다. 관리자가 Copilot Studio 통합 앱을 배포하지 않았거나 플러그인이 아직 인덱싱되지 않은 것일 수 있고, 따라서 잠시 기다려야 할 수도 있습니다.

2. Copilot Studio 섹션 아래의 작업 목록에서 **Professional Development Plan**이라는 이름의 작업을 찾고 옆에 있는 토글을 선택하여 사용하도록 설정합니다.

    > [!NOTE]
    > Copilot Studio의 플러그인 목록에 Professional Development Plan이 표시되지 않는 경우 표시하는 데 시간이 조금 더 걸릴 수 있습니다. Microsoft 365 Copilot에 표시하는 데에는 좀 더 걸릴 수 있습니다.

3. Professional Development Plan 작업을 사용하도록 설정한 후에는 이제 Copilot에서 사용할 수 있습니다. **체험**해 보기 위해 Teams의 Copilot에 다음 메시지를 보내 봅니다. "다음 경력 마일스톤을 달성하기 위해 전문성 개발 계획을 세우려고 해. 1 - 마케터로서의 업무 능력을 높이고 2 - 수석 마케터 역할로 승진할 가능성을 높이고 싶어."

**팁:** Copilot에서 개발자 모드를 사용하도록 설정하려면 채팅에 `-developer on`(이)라고 입력합니다.  이렇게 하면 Copilot이 채팅에서 응답하기 위해 플러그인을 사용했을 때 관찰할 수 있습니다.