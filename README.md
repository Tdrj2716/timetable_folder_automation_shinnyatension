# timetable_folder_automation_shinnyatension
KULASISのページから各講義のためのフォルダを作成します（forked from https://github.com/magochansan/timetable_folder_automation_shinnyatension ）

## How to use
gitとpython3が入っていることを前提にしています

1. リポジトリのclone（ここでは`create_timetable_folder`という名前でディレクトリを作成）
  ```sh
  git clone https://github.com/Tdrj2716/timetable_folder_automation_shinnyatension.git create_timetable_folder
  cd create_timetable_folder
  ```

2. 仮想環境の作成
  ```sh
  python -m venv .
  . bin/activate
  ```

3. 必要なパッケージのインストール

  ステップ2で作成された仮想環境下に、pythonで必要なパッケージをインストールします
  ```sh
  pip install -r requirements.txt
  ```

4. `.env`の作成

  ECS-IDとそのパスワード、及び各時間割のフォルダを配置するディレクトリのパス（`BASE_DIR`）を記述した`.env`ファイルを作成します。
  例（Mac, Linux）：
  ```.env
  ECS_ID = "a0123456"
  PASSWORD = "kulasis_pass"
  BASE_DIR = "/Users/usrname/Documents/B3-spring/"
  ```

5. プログラムの実行
  ```sh
  python main.py
  ```
