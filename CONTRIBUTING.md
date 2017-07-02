## How to Contribute

### Versioning
- [Semantic Versioning 2.0.0](http://semver.org/)에 따라 v{major}.{minor}.{hotfix} 형식을 사용한다.

### Branch
- [gitflow](http://danielkummer.github.io/git-flow-cheatsheet/index.ko_KR.html) model에 따라 나눈다.

- master : 가장 최근에 release 된 버전 / 직접커밋 금지
- hotfix : 긴급이슈 발생시 master로부터 hotfix branching 해서 배포함
- release/{major}.{minor}.{hotfix} : 배포를 하기위한 버전
- develop : 개발중인 버전
- feature/{xxx} : 각 feature 단위로 개발

### Commit
- (존재한다면) 관련 이슈를 referencing 한다.
- 제목과 본문을 빈 행으로 구분한다. 
- 형식 => {이슈번호} : {수정내용}

```
#1 : Create Skeleton Project 

- xxxx xxx
- xxx xxxx
```

### Pull Request
- 빠른 코드 리뷰가 가능하도록 PR 은 되도록 이슈 단위로 생성한다.
- Reviewer 를 assign 하기 전에, 해당 PR 로 인해 test 가 fail 되고 있진 않은지 확인한다.
- Reviewer는 최소한 2인 이상으로 한다.
  - Approve, Comment 는 담당자 판단하에 수정 여부를 결정하면 될만한 일반적인 feedback 을 의미한다.
  - Request changes 는 merge 이전에 reviewer 와 함께 고민해서 결론을 내야 하는 feedback 을 의미한다.
- **디자인 리뷰는 오프라인 or 행아웃으로 진행한다.**

### Coding Style
- [Databricks Scala Guide](https://github.com/databricks/scala-style-guide/blob/master/README-KO.md) 를 따른다.
- 그 외 [scala style checker](http://www.scalastyle.org/) 에서 요구하는 사항을 따른다.
