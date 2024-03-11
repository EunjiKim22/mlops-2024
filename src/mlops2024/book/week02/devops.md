# Week 2 - DevOps

![DevOps](figs/devops.jpeg)

DevOps는 소프트웨어 개발(Dev)과 IT 운영(Ops) 간의 격차를 해소하기 위한 실천 방법, 도구 및 문화적 철학의 조합입니다. DevOps의 주요 목표는 개발 및 운영 팀 간의 협업을 개선하고, 소프트웨어 개발 생명 주기를 간소화하며, 더 빠르고 안정적이며 높은 품질의 소프트웨어를 제공하는 것입니다.

DevOps는 여러 가지 핵심 원칙과 실천 방법을 포함합니다:

- **지속적 통합(CI)**: CI에서는 개발자가 코드 변경 사항을 공유 저장소에 자주 병합하며, 종종 하루에 여러 번 수행합니다. 각 통합 시 자동화된 빌드와 테스트가 실행되어 팀이 개발 프로세스 초기에 문제를 탐지하고 수정할 수 있습니다.

- **지속적 제공(CD)**: CD는 CI의 확장으로, 코드가 항상 릴리스 가능한 상태를 유지하는 것을 목표로 합니다. 이는 배포 프로세스를 자동화하고 최소한의 수동 개입으로 언제든지 소프트웨어를 프로덕션에 릴리스할 수 있도록 하는 것을 포함합니다.

- **코드로서의 인프라(IaC)**: IaC는 코드 및 버전 제어 시스템을 사용하여 인프라 리소스(네트워크, 서버, 스토리지 등)를 관리하고 프로비저닝하는 실천 방법입니다. 이를 통해 팀은 인프라 관리를 자동화하고, 일관성을 개선하며, 수동 오류를 줄일 수 있습니다.

- **모니터링 및 로깅**: 모니터링과 로깅은 애플리케이션 및 인프라에서 성능 메트릭, 로그 및 기타 데이터를 수집하고 분석하는 것을 포함합니다. 이는 팀이 문제를 식별하고, 문제를 해결하며, 성능을 최적화하는 데 도움이 됩니다.

- **협업 및 커뮤니케이션**: DevOps는 개발 및 운영 팀 간의 사일로를 타파하는 것을 강조합니다. 이는 개방적 커뮤니케이션 문화를 조성하고, 지식을 공유하며, 공동의 목표 달성을 위해 협력하는 것을 포함합니다.

- **피드백 및 지속적 개선**: DevOps는 학습, 실험 및 적응의 문화를 장려합니다. 팀은 다양한 출처(예: 모니터링, 사용자 피드백)에서 피드백을 수집하고 이 정보를 사용하여 프로세스, 도구 및 제품을 반복적으로 개선합니다.

![cicd](figs/cicd.jpeg)

최근에는 DevOps 분야에서 몇 가지 주목할 만한 발전이 있었습니다:

- **GitOps**: GitOps는 Git 저장소를 인프라 및 애플리케이션 구성의 단일 진실 공급원으로 사용하는 운영 모델입니다. 이를 통해 팀은 Git의 pull request 및 merge와 같은 친숙한 도구와 프로세스를 사용하여 인프라와 애플리케이션 변경 사항을 관리할 수 있습니다.

- **서버리스 컴퓨팅**: 서버리스 컴퓨팅은 개발자가 기본 인프라를 관리할 필요 없이 코드를 실행할 수 있는 클라우드 컴퓨팅 모델입니다. 이는 개발자가 애플리케이션 로직에 집중하고 인프라 관리의 복잡성을 줄일 수 있도록 해줍니다.

- **컨테이너 및 마이크로서비스**: 컨테이너와 마이크로서비스 아키텍처는 애플리케이션을 작고 독립적인 서비스로 분할하여 개발, 배포 및 확장을 더 쉽게 만듭니다. 이는 DevOps 팀이 애플리케이션 구성 요소를 더 효과적으로 관리하고 업데이트할 수 있도록 해줍니다.

- **AIOps**: AIOps(Artificial Intelligence for IT Operations)는 기계 학습과 빅데이터 분석을 사용하여 IT 운영을 자동화하고 최적화하는 것을 목표로 합니다. 이는 이상 탐지, 이벤트 상관 관계, 근본 원인 분석 등을 위해 AI를 활용하여 문제 해결 시간을 단축하고 시스템 성능을 개선하는 데 도움이 됩니다.

- **보안 및 규정 준수**: DevOps 팀은 DevSecOps 관행을 통해 개발 프로세스 전반에 걸쳐 보안과 규정 준수를 통합하는 데 점점 더 집중하고 있습니다. 여기에는 코드로서의 정책, 보안 테스트 자동화, 지속적인 모니터링 및 감사 등이 포함됩니다.

이러한 발전은 조직이 더 민첩하고 효율적이며 안전한 방식으로 소프트웨어를 제공할 수 있도록 지원하는 동시에 DevOps의 핵심 원칙과 실천 방법을 기반으로 합니다.

## DevOps의 작동 방식

DevOps는 이러한 목표를 달성하기 위해 도구, 방법론 및 문화적 변화와 같은 다양한 구성 요소를 통합하여 작동합니다.

DevOps가 작동하는 방식에 대한 개요는 다음과 같습니다:

- **문화 변화**: DevOps는 개발 및 운영 팀 간의 협업, 커뮤니케이션 및 공동 책임의 문화를 조성하는 것에서부터 시작됩니다. 이는 사일로를 타파하고, 개방적인 의사소통을 장려하며, 팀이 공통의 목표를 달성하기 위해 함께 일하는 환경을 조성하는 것을 포함합니다.

- **애자일 개발**: DevOps는 반복적 개발, 빈번한 릴리스 및 지속적인 개선을 촉진하는 애자일 방법론을 기반으로 합니다. 팀은 작고 기능 간 협력이 이루어지는 단위로 일하며, Scrum이나 Kanban과 같은 실천 방법을 따라 효율적으로 작업을 관리합니다.

- **지속적 통합(CI)**: CI는 개발자가 코드 변경 사항을 공유 저장소에 자주 병합하는 것을 포함하며, 종종 하루에 여러 번 이루어집니다. 각 통합 시 자동화된 빌드와 테스트가 실행되어 팀이 개발 프로세스 초기에 문제를 탐지하고 수정할 수 있습니다.

- **지속적 제공(CD)**: CD는 CI를 확장하여 코드가 항상 릴리스 가능한 상태를 유지하도록 합니다. 이는 배포 프로세스를 자동화하고 최소한의 수동 개입으로 소프트웨어를 프로덕션에 릴리스할 수 있도록 하는 것을 포함합니다.

- **코드로서의 인프라(IaC)**: IaC는 코드 및 버전 제어 시스템을 사용하여 인프라 리소스를 관리하고 프로비저닝하는 실천 방법입니다. 이를 통해 팀은 인프라 관리를 자동화하고, 일관성을 개선하며, 수동 오류를 줄일 수 있습니다.

- **자동화**: DevOps는 프로세스를 간소화하고 수동 작업을 줄이기 위해 자동화에 크게 의존합니다. 여기에는 빌드, 테스트, 배포, 인프라 프로비저닝 및 모니터링의 자동화가 포함됩니다.

- **모니터링 및 피드백**: DevOps는 애플리케이션 및 인프라에서 성능 메트릭, 로그 및 기타 데이터를 수집하고 분석하는 것을 강조합니다. 팀은 이 정보를 사용하여 문제를 파악하고, 문제를 해결하며, 성능을 최적화하고, 프로세스와 제품을 지속적으로 개선합니다.

- **지속적인 학습 및 개선**: DevOps는 학습, 실험 및 적응의 문화를 장려합니다. 팀은 다양한 출처(예: 모니터링, 사용자 피드백)의 피드백을 사용하여 프로세스, 도구 및 제품을 반복적으로 개선합니다.

최근 DevOps 분야에서는 다음과 같은 발전이 있었습니다:

- **GitOps**: GitOps는 Git 저장소를 인프라 및 애플리케이션 구성의 단일 진실 공급원으로 사용하는 운영 모델입니다. 이를 통해 팀은 Git의 풀 리퀘스트 및 병합과 같은 익숙한 도구와 프로세스를 사용하여 인프라와 애플리케이션 변경 사항을 관리할 수 있습니다.

- **사이트 안정성 엔지니어링(SRE)**: SRE는 소프트웨어 엔지니어링 원칙을 IT 운영에 적용하여 시스템 안정성과 성능을 개선하는 것을 목표로 합니다. DevOps 팀은 SRE 실천 방법을 도입하여 시스템 신뢰성을 높이고, 인시던트 대응 시간을 단축하며, 운영 효율성을 개선하고 있습니다.

- **프로그레시브 딜리버리**: 프로그레시브 딜리버리는 기능 플래그, 카나리아 릴리스, A/B 테스팅과 같은 기술을 사용하여 새로운 기능을 점진적으로 롤아웃하고 사용자 피드백을 수집하는 것을 포함합니다. 이를 통해 팀은 위험을 최소화하면서 혁신을 가속화할 수 있습니다.

- **ObservabilityOps**: ObservabilityOps는 애플리케이션 및 인프라 동작에 대한 심층적인 통찰력을 얻기 위해 메트릭, 로그 및 트레이스를 사용하는 것을 강조합니다. 이는 DevOps 팀이 문제를 더 빠르게 해결하고, 성능을 최적화하며, 사용자 경험을 개선하는 데 도움이 됩니다.

이러한 발전은 DevOps의 핵심 원칙과 실천 방법을 기반으로 하여 조직이 더 민첩하고, 안정적이며, 고객 중심적인 방식으로 소프트웨어를 제공할 수 있도록 지원합니다.

## DevOps 도구

소프트웨어 개발 및 운영 프로세스의 다양한 측면을 자동화하고 간소화하는 데 도움이 되는 다양한 DevOps 도구가 있습니다. 이러한 도구는 협업, 지속적 통합 및 제공, 인프라 관리, 모니터링 등을 지원합니다. 다음은 카테고리별로 그룹화된 인기 있는 DevOps 도구 목록입니다:

### 버전 제어:

- **Git**: 협업을 가능하게 하고 코드베이스의 변경 사항을 추적하는 널리 사용되는 분산 버전 제어 시스템입니다.

- **GitHub, GitLab, Bitbucket**: Git 저장소 호스팅, 이슈 추적 및 협업 기능을 제공하는 웹 기반 플랫폼입니다.

### 지속적 통합 및 지속적 제공(CI/CD):

- **Jenkins**: 코드 변경 사항 빌드, 테스트 및 배포를 지원하는 오픈 소스 자동화 서버입니다.

- **GitLab CI/CD**: GitLab 내에 내장된 CI/CD 솔루션으로 파이프라인 관리 및 자동화를 제공합니다.

- **GitHub Actions**: GitHub 저장소와 통합되고 워크플로우 자동화를 지원하는 CI/CD 솔루션입니다.

- **CircleCI**: 파이프라인 설정 및 관리를 단순화하는 클라우드 기반 CI/CD 플랫폼입니다.

- **Travis CI**: 인기 있는 버전 제어 시스템과 통합되는 또 다른 클라우드 기반 CI/CD 서비스입니다.

- **Bamboo**: Jira 및 Bitbucket과 같은 다른 Atlassian 도구와 통합되는 Atlassian의 온프레미스 CI/CD 솔루션입니다.

### 구성 관리 및 코드로서의 인프라(IaC):

- **Ansible**: 자동화를 위해 간단하고 사람이 읽을 수 있는 언어(YAML)를 사용하는 오픈 소스 구성 관리 및 애플리케이션 배포 도구입니다.

- **Puppet**: 인프라 리소스를 관리하기 위해 선언적 언어(Puppet DSL)를 사용하는 구성 관리 도구입니다.

- **Chef**: 인프라 자동화를 위해 Ruby 기반 도메인 특화 언어(DSL)를 사용하는 또 다른 구성 관리 도구입니다.

- **SaltStack**: 자동화를 위해 Python 기반 DSL과 YAML을 사용하는 구성 관리 및 원격 실행 도구입니다.

- **Terraform**: 다양한 클라우드 플랫폼에서 인프라를 프로비저닝하고 관리하기 위한 HashiCorp의 오픈 소스 IaC 도구입니다.

### 컨테이너화 및 오케스트레이션:

- **Docker**: 일관되고 재현 가능한 환경을 활성화하는 컨테이너를 사용하여 애플리케이션 패키징 및 배포를 단순화하는 플랫폼입니다.

- **Kubernetes**: 컨테이너화된 애플리케이션의 배포, 스케일링 및 관리를 자동화하기 위한 컨테이너 오케스트레이션 플랫폼입니다.

- **Helm**: Kubernetes 클러스터에 애플리케이션을 배포하고 관리하는 데 도움이 되는 Kubernetes용 패키지 관리자입니다.

- **OpenShift**: Kubernetes 위에 구축된 Red Hat의 컨테이너 플랫폼으로, 엔터프라이즈 사용 사례를 위한 추가 기능 및 통합을 제공합니다.

### 모니터링 및 로깅:

- **Prometheus**: 다양한 소스에서 시계열 메트릭을 수집하고 저장하는 오픈 소스 모니터링 및 경고 도구입니다.

- **Grafana**: Prometheus, Elasticsearch 등을 포함한 여러 데이터 소스를 지원하는 시각화 및 분석 플랫폼입니다.

- **ELK 스택(Elasticsearch, Logstash, Kibana)**: 중앙 집중식 로깅, 로그 처리 및 로그 분석을 위한 도구 모음입니다.

- **Datadog**: 애플리케이션, 인프라 및 로그에 걸친 전체 스택 가시성을 제공하는 클라우드 기반 모니터링 및 분석 플랫폼입니다.

- **Splunk**: 실시간 모니터링 및 경고를 지원하는 로그 관리, 분석 및 시각화 플랫폼입니다.

이는 사용 가능한 많은 DevOps 도구 중 몇 가지 예시일 뿐입니다. 조직에 맞는 도구를 선택할 때는 사용 편의성, 기존 시스템과의 통합, 확장성, 개발 및 운영 프로세스의 특정 요구사항 등의 요소를 고려해야 합니다.

최근의 DevOps 도구 동향을 살펴보면 다음과 같은 발전이 있습니다:

- **GitOps 도구**: ArgoCD, Flux, Jenkins X 등의 도구는 Git 저장소를 사용하여 인프라 및 애플리케이션 구성을 관리하고 배포 프로세스를 자동화합니다.

- **서버리스 및 FaaS(Function as a Service) 도구**: AWS Lambda, Google Cloud Functions, Azure Functions 등의 도구는 서버리스 애플리케이션 개발 및 배포를 지원하여 인프라 관리 부담을 줄입니다.

- **AIOps 도구**: Dynatrace, New Relic, PagerDuty 등의 도구는 AI와 기계 학습을 활용하여 이상 탐지, 근본 원인 분석, 인시던트 대응을 자동화합니다.

- **보안 및 규정 준수 도구**: HashiCorp Vault, Aqua Security, Snyk 등의 도구는 보안과 규정 준수를 DevOps 프로세스에 통합하는 데 도움이 됩니다.

- **Value Stream Management(VSM) 도구**: Tasktop, Plutora, CloudBees 등의 도구는 엔드-투-엔드 소프트웨어 딜리버리 프로세스를 시각화, 측정 및 최적화하여 효율성과 가치 창출을 개선합니다.

이러한 도구들은 DevOps 팀이 소프트웨어 제공 프로세스를 더욱 자동화, 간소화 및 최적화할 수 있도록 지원하여 더 빠르고, 안정적이며, 고객 중심적인 애플리케이션을 개발할 수 있도록 도와줍니다.

```{tableofcontents}

```