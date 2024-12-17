closes `#123`

```
## 변경 사항

### 1. SQLite 데이터베이스 위치 변경
- **파일**: [coinpan-bot/coinpan/data/sqlite/sqlitehandler.py](cci:7://file:///home/user/codes/coinpan/coinpan-bot/coinpan/data/sqlite/sqlitehandler.py:0:0-0:0)
  - 데이터베이스 파일 경로를 `~/.coinpan/coinpan.db`에서 프로젝트 루트의 `database/coinpan.db`로 변경
  - 사용하지 않는 [os](cci:1://file:///home/user/codes/coinpan/coinpan-bot/coinpan/data/sqlite/sqlitehandler.py:52:4-56:40) import 제거

### 2. 테스트 데이터베이스 위치 변경
- **파일**: [coinpan-bot/tests/conftest.py](cci:7://file:///home/user/codes/coinpan/coinpan-bot/tests/conftest.py:0:0-0:0)
  - 테스트 데이터베이스 파일 경로를 `~/.coinpan/test/test.db`에서 프로젝트 루트의 `database/test.db`로 변경

### 3. .gitignore 업데이트
- **파일**: [.gitignore](cci:7://file:///home/user/codes/coinpan/.gitignore:0:0-0:0)
  - `*.db` 패턴 추가하여 모든 데이터베이스 파일을 git에서 제외

## 요약
데이터베이스 파일들을 프로젝트 루트의 `database` 디렉토리에서 관리하도록 변경하고, 이를 git에서 제외하도록 설정했습니다. 이를 통해 데이터베이스 파일 관리가 더 명확해지고, 실수로 데이터베이스 파일이 git에 커밋되는 것을 방지할 수 있습니다.
```
