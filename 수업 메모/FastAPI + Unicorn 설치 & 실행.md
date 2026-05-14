## 260507

1. **새로운 파일 생성 `requirements.txt`**
![[image.png]]

2. **cursor 터미널 열어 한줄씩 복붙**
-> if (!(Test-Path $PROFILE)) { New-Item -Type File -Path $PROFILE -Force }
-> notepad $PROFILE

3. **창에 뜬 메모장에 아래 글 복붙**
#.프로젝트 루트로 이동 cloud.cloverky 부분은 자기 폴더 있는 위치로 변경
Set-Location "C:\Users\hi\Documents\cloud.cloverky" 
#.venv 활성화 (있을 때만)
$venvActivate = "C:\Users\hi\Documents\cloud.cloverky\.venv\Scripts\Activate.ps1"
if (Test-Path $venvActivate) {
    & $venvActivate
}

4. **저장 후 윈도우 키 눌러 powershell 우클릭 관리자로 실행 후 아래 글 복붙**
Set-ExecutionPolicy -Scope CurrentUser RemoteSigned
+모두 허용 S 입력

5.  **새 powershell 열어 아래 글 복붙**
Get-Location"
python -c "import sys; print(sys.executable)

6. **cursor에 들어가서 requirements.txt 파일을 끌어다 놓고 Agent로 변경 후에 아래 글 복붙**
`requirements.txt` 여기에 FastAPI uvicorn pandas 를 등록해줘 