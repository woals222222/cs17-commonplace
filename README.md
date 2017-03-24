# cs17-commonplace

이 repository는 2017년 1학기 서울대학교 M1399.000100 통계계산 과목을 위한 repository입니다. 이 곳을 아래의 기능을 수행합니다.

* 공지사항
* 강의노트 게시
* 질의 응답(이슈 트래커 사용)
* 숙제 안내

이 repository는 수강생 전체에게 공개되며, 이슈 트래커를 통해 논의를 진행하기를 권장합니다. 

* 이곳의 이슈 트래커를 통해 숙제에 관한 활발한 논의를 진행하는 것을 장려하나, __숙제 코드 또는 답안의 일부를 직접 올려서는 안 됩니다__.
  * 단, 강의록이나 숙제 문제지, 또는 조교를 통해 배포된 코드는 그대로 올려 논의해도 무방합니다.
* 숙제 보고서 작성 이 곳에서 논의된 내용을 참고한 경우 숙제에 issue 번호를 기록하면 됩니다.
* 다른 사람에게 공개하기를 원하지 않는 질문은 개인 숙제 제출 repository의 이슈 트래커에서 할 수 있습니다.
* 자주 나오는 질문은 위키 또는 이슈 트래커를 통해 따로 공지할 수 있습니다.
* 숙제 제출 전 다음 내용을 숙지하시기 바랍니다.

## 숙제 진행

1. 숙제 출제 시 url 링크 하나가 함께 공개됩니다. 이 링크를 통해 개인 별 숙제 제출을 위한 repository를 생성합니다.
1. 생성된 repository에는 여러분이 직접 편집할 수 있습니다. git, GitHub Desktop을 사용하거나 GitHub 홈페이지에서 직접 파일으르 업로드할 수 있습니다.
1. 채점 대상은 `master` 브랜치에 있는 내용입니다.
1. 숙제 마감 시점이 되면 자동으로 여러분의 repository를 clone하여 서버에 저장합니다. 이후 push한 내용은 _채점에 반영되지 않습니다._

### 숙제 링크

* [숙제 0](https://classroom.github.com/assignment-invitations/8634c9b1ff9f4c13e8ef22437577ae0a): 숙제 제출 연습 및 계정 정보 제출. 3월 26일 23:59 마감.
* [숙제 1](https://classroom.github.com/assignment-invitations/888ad5c92b022a79a710d600b2281416): 3월 31일 23:59 마감.
* 숙제 2: 
* 숙제 3:
* 숙제 4:

## 제출 내용

보고서 파일, 보고서 작성을 위해 사용한 파일, 문제 풀이에 사용한 소스 코드를 각각 제출해야 합니다. 파일 크기 제한은 GitHub의 기본 제한(파일 하나 당 100MB, repository 전체 1GB)을 따릅니다.

### 보고서 파일 (`doc/`)

* 모든 채점의 기준이 되며, 작성 방식에는 따로 제약이 없습니다.
* 보고서 파일에는 문제풀이와 코드 실행 결과가 _정리되어_ 있어야 합니다. 
* 최대 **두 개**의 `pdf` 또는 `html` 파일이 허용됩니다.
* `html` 또는 `ipynb` 파일을 사용하는 경우 그림 파일이 제대로 표시되는 지 확인하시기 바랍니다. [상대 경로](https://en.wikipedia.org/wiki/Path_(computing)#Absolute_and_relative_paths)를 활용해 주세요. 
* 손으로 쓴 내용을 스캔하는 경우 조교가 알아볼 수 있을 정도의 해상도를 사용하기 바랍니다.

### 문서 작성을 위해 사용한 파일 (`doc/`)

* 위에 적힌 형식의 파일을 만들기 위해 사용한 __모든__ 파일
* `.doc`, `.docx`, `.hwp`, `.Rmd`, `.md` 등등
* 설명이 필요하다고 판단되는 경우 작성 방법에 대해서도 기록할 것.

### 문제 풀이에 사용한 소스 코드 (`src/`)

* `.R`, `.py`, `.c` 등등. 오픈 소스이거나 학교가 라이센스를 보유한 프로그램이면서 조교가 이해할 수 있는 언어를 사용하면 됩니다. 아래 목록에 포함되지 않은 언어를 사용하고자 하는 경우 조교에게 문의하기 바랍니다.
  * R, Python, Fortran, C, C++, Java, Scala, Julia, Matlab, Octave
* 코드에는 이해를 돕기 위해 충분한 주석이 달려 있어야 합니다.
* 코드는 문항 별, 또는 적절한 단위로 파일을 나누어 제출해야 합니다. 예를 들어, R을 사용하는 경우 `source` 함수 또는 `Rscript` 프로그램을 사용하여 원하는 문항에 해당하는 부분만 따로 실행할 수 있어야 합니다.
* 일부 문항은 별도의 데이터 파일을 입력받아 사용해야 합니다. 이 때 절대 경로가 아닌 [상대 경로](https://en.wikipedia.org/wiki/Path_(computing)#Absolute_and_relative_paths)를 사용해야 합니다.
* 함수를 구현하는 문항의 경우 다른 문항에서 그 함수를 사용하지 않으면 해당 함수가 잘 구현되었는지 확인하기 위한 테스트 코드와 그 결과를 첨부해야 합니다.
* 문서 파일에 첨부된 결과를 재현할 수 있어야 합니다.
  * 시뮬레이션 문제의 경우, R의 `set.seed`와 같이 같은 결과를 재현할 수 있게 해 주는 설정을 사용해야 합니다.
  * R Markdown Notebook을 사용하는 경우, 첫 번째 chunk부터 차례대로 실행했을 때 보고서와 같은 결과가 나와야 합니다.
* R Markdown Notebook, Jupyter Notebook, Matlab Live Script를 사용하는 경우 소스 코드를 따로 첨부하지 않을 수 있습니다. 단, 보고서 `.html`, `.pdf` 파일은 제출해야 합니다.

### `README.md`

다음과 같은 내용을 포함해야 합니다.

* 학번, 이름
* 제출 파일의 간단한 설명
  * 보고서 파일이 어떤 파일인지 명시할 것.
* 보고서 작성 방법
* 코드 컴파일 또는 실행 방법 (따로 설명이 필요한 경우)

## 문서 작성하기
R이나 다른 스크립트 언어 실행 결과와 latex 문법, 마크다운을 결합하여 문서를 만드는 방법에는 여러 가지가 있으며, 이들 중 마음에 드는 것을 골라 사용하기를 권장합니다. 특히, 최신 버전 [RStudio](https://rmarkdown.rstudio.com/)에서 쓸 수 있는 [R Markdown Notebook](https://rmarkdown.rstudio.com/r_notebooks.html)은 [문학적 프로그래밍(literate programming)](http://www2.warwick.ac.uk/fac/sci/wdsi/vacationschool2016/for-participants/materials/LitProg.pdf) 방식의 일종으로서 html 형식 보고서 작성이 수월해질 것입니다. 

## 추가 사항 
* 다른 사람과 구두로 또는 cs17-commonplace의 이슈 트래커를 통해 논의할 수 있습니다. 과제 레포트의 해당 부분에 함께 논의한 학생 이름과 어떤 부분을 논의했는지 기록해야 합니다. 이슈 트래커에서 논의한 내용을 사용할 경우 해당 이슈 번호를 기입하면 됩니다. 
* 다른 사람과 코드와 작성된 레포트를 공유하면 안 됩니다. 다른 사람의 코드/레포트를 베끼는 것도, 다른 사람에게 코드/레포트를 보여주는 것도 모두 심각한 부정행위로 간주됩니다. 숙제 문제 또는 답안을 public repository에 공개해서도 안 됩니다. 

## 페널티
* 형식 오류
  * 첫 번째 숙제에서는 형식 오류로 인한 페널티가 부과되지 않습니다.
  * 두 번째 숙제부터는 형식 오류 정도에 따라 최대 만점의 10%까지의 페널티가 부과될 수 있습니다.
* 표절/공유
  * 해당 숙제 0점 처리, 심한 경우 F학점 부여. 

