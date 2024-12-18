# Fitness App

이 프로젝트는 Android용 간단한 피트니스 앱 예제입니다.  
사용자는 회원가입 및 로그인 후, 자신만의 운동 루틴을 생성하고, 루틴에 운동을 추가 및 관리할 수 있습니다. 또한 각 운동에 대한 상세정보를 확인할 수 있습니다.

## 주요 기능

- **회원가입 및 로그인**: 사용자 정보(이름, 나이, 키, 몸무게, ID, PW)를 이용해 회원가입 가능.
- **루틴 생성 및 관리**: 
  - 새로운 루틴을 생성할 수 있고, 
  - 생성한 루틴의 이름을 수정하거나 삭제할 수 있습니다.
- **운동 추가 및 관리**: 
  - 운동 목록에서 원하는 운동을 루틴에 추가.
  - 운동 아이템을 길게 눌러 루틴에서 해당 운동을 제거.
  - 운동명을 클릭하여 운동에 대한 상세정보(에너지소비량, 유형) 확인.

## 파일 구조

- `app/src/main/java/kr/co/softcampus/firnessapp/`
  - `LoginActivity.java`: 로그인 화면 액티비티
  - `RegisterActivity.java`: 회원가입 화면 액티비티
  - `MainActivity.java`: 메인 화면, 현재 사용자에 대한 인사말 및 루틴 선택 UI
  - `RoutineListActivity.java`: 사용자의 루틴 목록 관리 화면
  - `CreateRoutineActivity.java`: 새로운 루틴을 생성하는 화면
  - `RoutineDetailActivity.java`: 특정 루틴에 대한 상세 화면(운동 목록 관리)
  - `SelectExerciseActivity.java`: 운동 목록에서 루틴에 운동을 추가하는 화면
  - `ExerciseDetailActivity.java`: 특정 운동에 대한 상세정보를 보여주는 화면
  - `DBHelper.java`: SQLite DB 관리 헬퍼 클래스, 사용자/루틴/운동 데이터 관리 로직 포함
  - `User.java`, `Routine.java`, `Exercise.java`, `RoutineExercise.java`: 데이터 모델 클래스들
  
- `app/src/main/res/layout/`
  - `activity_login.xml`, `activity_register.xml`, `activity_main.xml`, `activity_routine_list.xml`, `activity_create_routine.xml`, `activity_routine_detail.xml`, `activity_select_exercise.xml`, `activity_exercise_detail.xml`: 각 액티비티에 해당하는 레이아웃 파일
  
- `AndroidManifest.xml`: 액티비티 등록 및 앱 권한 설정


## 초기 세팅

### 요구사항
- Android Studio (Arctic Fox 이상 권장)
- Android SDK 31 이상
- JDK 11 이상 (Android Studio 통합 JDK 사용 권장)

### 빌드/실행 방법
1. 저장소를 로컬에 클론합니다.
   ```bash
   git clone https://github.com/yourusername/fitnessapp.git
