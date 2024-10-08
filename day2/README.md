- 과제에서 사용하는 리전은 현장에서 나눠준 문제지에 적힌 리전을 사용해야 합니다. **반드시** 사용하는 리전을 꼭 확인 후 리소스를 생성 하도록 합니다.
- Bastion을 알아서 생성 하도록 되어 있는 과제들이 있는데 각 Bastion은 각각 생성하고 심사시 알아볼 수 있도록 태그를 추가해둡니다. `예) bastion-eks_observ`
- VPC 사용에 대한 언급이 없으면 새로운 VPC 생성을 권장합니다. 다만 선수가 채점에 이상이 없을거라고 판단 되면 기본 VPC를 사용해도 무방합니다.
- 부산 CloudTrail을 사용하는 거너넌스 과제의 경우 en-central-1을 사용하는 단독과제 임으로 기본 VPC를 사용해도 무방합니다.
- 충남 거버넌스 과제의 경우 ap-southeast-1을 사용하는 단독과제 임으로 문제에 명시된 대로 기본 VPC를 사용합니다.
- 충남 거버넌스 과제에서 생성하는 IAM user Admin이 기본 과제의 IAM 유저 admin과 겹침으로 과제의 유저는 myadmin `(소문자)`로 변경하여 구성 합니다. 기타 다른 과제에서도 admin IAM 유저와 겹친다면 모두 myadmin으로 변경합니다.
- Client VPN 문제에서 CIDR에 태그를 추가하는 케이스는 없습니다. CIDR은 그림을 참고하고 VPC에는 Name 태그를 추가 하라는 의미입니다.
- 각 모듈별 Bastion에서 채점 하는 경우 awscli에서 region 지정에 문제가 없도록 `.aws/config` 파일에 region 구성을 잘 해두도록 합니다.
