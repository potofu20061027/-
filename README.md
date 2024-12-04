README for Fourier analysis and waveform editing of audio files

必要なライブラリ:
pip install pydub matplotlib numpy scipy

google colabでの使用を想定しています。

使い方
1. 音声ファイルのアップロード
最初に、処理したい音声ファイル（対応するファイル形式:入力はMP3またはWAV形式の音声ファイル。処理後の音声はMP3形式で保存されます。）をアップロードします。

3. 音声データの処理
処理のオプションとして、以下の3つの処理を選択できます。

オプション1: (指定)Hz以下20Hz以上の部分の振幅を(指定)倍にする
オプション2: 振幅の上位何%までの周波数を残す
オプション3: 100Hz以下と1000Hz以上を0.7倍、それ以外の部分を1.3倍にする
ユーザーがこれらの処理を選択し、適用することができます。処理後は、スペクトルと波形が表示され、納得がいけば処理を完了し、MP3ファイルとしてダウンロードできます。

3. 処理の繰り返し
処理後、再度同じファイルで処理をやり直すことができます。繰り返し処理を行い、最適な結果を得ることができます。

4. ダウンロード
最終的に処理された音声データをMP3ファイルとしてダウンロードすることができます。


README Fourier analysis and waveform editing of audio files

Required Libraries:
pip install pydub matplotlib numpy scipy

Usage
1. Upload an Audio File
First, upload the audio file you want to process (MP3 or WAV). Before uploading, choose the format (MP3 or WAV) for processing.

2. Audio Data Processing
After uploading the file, you can select from the following three processing options:

Option 1: Amplify the frequencies within a specified range (e.g., increase the amplitude of frequencies below (specified) Hz and above (specified) Hz).
Option 2: Retain the top N% of frequencies based on amplitude.
Option 3: Reduce frequencies below 100Hz and above 1000Hz by 0.7 times, and increase the other frequencies by 1.3 times.
The user can select and apply any of these processing options. After processing, the spectrum and waveform of the audio will be displayed. If satisfied with the results, the user can finalize the processing and download the audio file in MP3 format.

3. Repeat Processing
After processing, you can choose to reprocess the same file. You can fine-tune the processing until you are satisfied with the results.

4. Download
Once the audio is processed to your satisfaction, you can download the final MP3 file.


README for Fourier series expansion

必要なライブラリ:
pip install gspread matplotlib numpy scipy oauth2client

使い方
使用にはフーリエ級数展開についての基本的な知識を要求します。

1. Google スプレッドシートからデータを取得
最初に、処理したいGoogle スプレッドシートのURLを入力します。このシートからxとyのデータを取得します。

2. 近似曲線の作成
取得したデータを元に、指定した次数で近似曲線を作成します。次数はユーザーが入力します。

3. 高速フーリエ変換とスペクトル解析
近似曲線に基づいて、スペクトルを計算します。
計算したスペクトルのa(n)とb(n)を表形式で表示します。
a(n)とb(n)の振幅をそれぞれプロットして表示します。
4. 結果の表示
近似曲線とそのスペクトルをプロットで確認し、計算結果を表示します。


README for Fourier series expansion

Required Libraries:
pip install gspread matplotlib numpy scipy oauth2client

Usage
Requires basic knowledge of Fourier series expansion.

1. Retrieve Data from Google Sheets
First, enter the URL of the Google Spreadsheet you want to process. Data from this sheet (x and y values) will be retrieved.

2. Create Fitted Curve
Using the data, a fitted curve will be created with a degree of approximation specified by the user. You can enter the degree of the polynomial.

3. Fast Fourier Transform and Spectrum Analysis
Based on the fitted curve, the spectrum will be calculated.
The calculated a(n) and b(n) values will be displayed in a table format.
The amplitudes of a(n) and b(n) will be plotted.
4. Display Results
The fitted curve and its spectrum will be displayed in plots, and the results will be shown.
