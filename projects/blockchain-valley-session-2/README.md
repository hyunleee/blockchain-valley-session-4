# 🎓 블록체인 밸리 X 알고랜드 개발자 부트캠프

## 🚩 세션 1: 알고킷 유틸리티 라이어버리를 사용해 여러 트랜잭션을 보내보자!

첫번째 알고랜드 개발자 부트캠프에 오신 블록체인 밸리 학회원분들 반갑습니다~!

세부 일정:

1. 알고랜드 기초 개념 알아보기 (30분)
2. 코드 데모: algokit utils typescript를 사용해서 알고 송금하는법 배우기 (30분)
3. 코딩 세션: 여러 알고랜드 기능들과 트랜잭션을 활용해서 특정 시나리오 구축해보기 (2시간)

이번 코딩 세션에서는 다음과 같은 시나리오를 [algokit utils typescript](https://github.com/algorandfoundation/algokit-utils-ts) 라이브러리를 사용해서 구현해보겠습니다.

시나리오:
앨리스는 애플 비전 프로가 너무 사고싶었지만 한국에서는 팔지 않아서 미국에 있는 크리스에게 대신 사달라고 부탁하기로 합니다.
크리스는 앨리스에게 애플 비전 프로를 사주는 대신 이자 10%를 달라고 요구했습니다.
앨리스는 크리스의 조건에 동의했고 크리스는 앨리스 대신 밥으로 부터 애플 비전 프로를 구매하기로 합니다. 밥은 크리스에게로부터
돈을 받으면 앨리스에게 애플 비전 프로를 보내겠다고 합니다.
이렇게 3자 거래가 성립되었습니다. 이 거래가 공정하게 이루어지려면 꼭 3개의 트랜잭션이 동시에 체결되어야 합니다.

이 상상의 세계에서는 비전 프로의 가격은 100 ALGO입니다 (부럽다... ㅠ\_ㅠ)

코딩 과제는 총 5문제로 구성되어 있으며 각 문제에 "**_ 여기에 코드 작성 _**" 부분에 코드를 작성하시면 됩니다. 밑에 체크포인트들을 따라서 진행해주세요.

## 체크포인트 1: 🧰 알고랜드 개발에 필요한 툴킷 설치

1. [AlgoKit 설치](https://github.com/algorandfoundation/algokit-cli/tree/main?tab=readme-ov-file#install).
2. [Docker 설치](https://www.docker.com/products/docker-desktop/). It is used to run a local Algorand network for development.
3. [Node.JS / npm 설치](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm)

## 체크포인트 2: 💻 개발 환경 셋업

1. [이 리포를 fork 해주세요.](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/fork-a-repo)
2. Fork한 리포를 git clone 해주세요.

```bash
cd [DIRECTORY_OF_YOUR_CHOICE]
git clone [FORKED_REPO_URL]
```

3. VSCode에서 이 폴더를 열람해주세요.
4. 열람 후 VSCode 터미널에서 `algokit project bootstrap all` 커맨드를 실행시켜 dependencies들을 설치해주세요.

```bash
algokit project bootstrap all
```

리포 fork, clone 튜토리얼:
https://github.com/algorand-fix-the-bug-campaign/challenge-1/assets/52557585/acde8053-a8dd-4f53-8bad-45de1068bfda

## 체크포인트 3: 📝 문제를 해결하세요!

1. 도커 데스크탑을 실행한 뒤 터미널에서 `algokit localnet start` 커맨드로 로컬 네트워크를 실행시켜주세요.[더 자세히 알고 싶다면 여기를 클릭해주세요!](https://github.com/algorandfoundation/algokit-cli/blob/main/docs/features/localnet.md#creating--starting-the-localnet).
2. `index.ts` 파일로 가셔서 설명을 읽으시고 문제들을 해결해보세요.
3. 문제를 다 해결한 뒤 터미널에서 `npm run start` 커맨드를 실행하시면 `index.ts` 파일을 실행하실 수 있습니다.
   실행 후 다음과 같은 콘솔 값이 출력되면 성공적으로 모든 문제를 해결하신겁니다!

![alt text](image.png)

**😰 힌트가 필요하신가요?**
알고랜드 클라이언트 기능들: https://github.com/algorandfoundation/algokit-utils-ts/blob/main/docs/code/classes/types_algorand_client.AlgorandClient.md

## 체크포인트 4: 💯 과제 제출하는 방법

1. 성공적으로 다섯 문제를 해결한 후 본인이 fork한 깃헙 리포로 코드를 푸쉬해주세요. 그런 다음 [원래의 리포로 Pull request를 해주세요.](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request-from-a-fork)
2. Pull Request 할때 `index.ts`를 실행시켜 출력된 값을 보여주는 터미널의 스크린샷을 첨부해주세요.

# blockchain-valley-session-2

This project has been generated using AlgoKit. See below for default getting started instructions.

# Setup

### Pre-requisites

- [Python 3.12](https://www.python.org/downloads/) or later
- [Docker](https://www.docker.com/) (only required for LocalNet)

> For interactive tour over the codebase, download [vsls-contrib.codetour](https://marketplace.visualstudio.com/items?itemName=vsls-contrib.codetour) extension for VS Code, then open the [`.codetour.json`](./.tours/getting-started-with-your-algokit-project.tour) file in code tour extension.

### Initial Setup

#### 1. Clone the Repository

Start by cloning this repository to your local machine.

#### 2. Install Pre-requisites

Ensure the following pre-requisites are installed and properly configured:

- **Docker**: Required for running a local Algorand network. [Install Docker](https://www.docker.com/).
- **AlgoKit CLI**: Essential for project setup and operations. Install the latest version from [AlgoKit CLI Installation Guide](https://github.com/algorandfoundation/algokit-cli#install). Verify installation with `algokit --version`, expecting `2.0.0` or later.

#### 3. Bootstrap Your Local Environment

Run the following commands within the project folder:

- **Install Poetry**: Required for Python dependency management. [Installation Guide](https://python-poetry.org/docs/#installation). Verify with `poetry -V` to see version `1.2`+.
- **Setup Project**: Execute `algokit project bootstrap all` to:
  - Install dependencies and setup a Python virtual environment in `.venv`.
  - Copy `.env.template` to `.env`.
- **Start LocalNet**: Use `algokit localnet start` to initiate a local Algorand network.

### Development Workflow

#### Terminal

Directly manage and interact with your project using AlgoKit commands:

1. **Build Contracts**: `algokit project run build` compiles all smart contracts.
2. **Deploy**: Use `algokit project deploy localnet` to deploy contracts to the local network.

#### VS Code

For a seamless experience with breakpoint debugging and other features:

1. **Open Project**: In VS Code, open the repository root.
2. **Install Extensions**: Follow prompts to install recommended extensions.
3. **Debugging**:
   - Use `F5` to start debugging.
   - **Windows Users**: Select the Python interpreter at `./.venv/Scripts/python.exe` via `Ctrl/Cmd + Shift + P` > `Python: Select Interpreter` before the first run.

#### JetBrains IDEs

While primarily optimized for VS Code, JetBrains IDEs are supported:

1. **Open Project**: In your JetBrains IDE, open the repository root.
2. **Automatic Setup**: The IDE should configure the Python interpreter and virtual environment.
3. **Debugging**: Use `Shift+F10` or `Ctrl+R` to start debugging. Note: Windows users may encounter issues with pre-launch tasks due to a known bug. See [JetBrains forums](https://youtrack.jetbrains.com/issue/IDEA-277486/Shell-script-configuration-cannot-run-as-before-launch-task) for workarounds.

## AlgoKit Workspaces and Project Management

This project supports both standalone and monorepo setups through AlgoKit workspaces. Leverage [`algokit project run`](https://github.com/algorandfoundation/algokit-cli/blob/main/docs/features/project/run.md) commands for efficient monorepo project orchestration and management across multiple projects within a workspace.

> For guidance on `smart_contracts` folder and adding new contracts to the project please see [README](smart_contracts/README.md) on the respective folder.

# Tools

This project makes use of Algorand Python to build Algorand smart contracts. The following tools are in use:

- [Algorand](https://www.algorand.com/) - Layer 1 Blockchain; [Developer portal](https://developer.algorand.org/), [Why Algorand?](https://developer.algorand.org/docs/get-started/basics/why_algorand/)
- [AlgoKit](https://github.com/algorandfoundation/algokit-cli) - One-stop shop tool for developers building on the Algorand network; [docs](https://github.com/algorandfoundation/algokit-cli/blob/main/docs/algokit.md), [intro tutorial](https://github.com/algorandfoundation/algokit-cli/blob/main/docs/tutorials/intro.md)
- [Algorand Python](https://github.com/algorandfoundation/puya) - A semantically and syntactically compatible, typed Python language that works with standard Python tooling and allows you to express smart contracts (apps) and smart signatures (logic signatures) for deployment on the Algorand Virtual Machine (AVM); [docs](https://github.com/algorandfoundation/puya), [examples](https://github.com/algorandfoundation/puya/tree/main/examples)
- [AlgoKit Utils](https://github.com/algorandfoundation/algokit-utils-ts) - A set of core Algorand utilities that make it easier to build solutions on Algorand.
- [Poetry](https://python-poetry.org/): Python packaging and dependency management.
- [npm](https://www.npmjs.com/): Node.js package manager
- [TypeScript](https://www.typescriptlang.org/): Strongly typed programming language that builds on JavaScript
- [ts-node-dev](https://github.com/wclr/ts-node-dev): TypeScript development execution environment

It has also been configured to have a productive dev experience out of the box in [VS Code](https://code.visualstudio.com/), see the [.vscode](./.vscode) folder.