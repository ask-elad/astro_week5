## Astro Sonification Utility tool

**Introduction**

Technical documentation for the Image Sonification Utility.

**Project Structure**

In the Main file:

1. main.py
2.requirements.txt
3. README.txt
4. images.npy(sampleset)
5. output: i. data.csv(example) ii. sound.wav(example)
6. utils: i. data_to_csv.py ii.sonification.py

**Installation**

1.  `git clone <repository_url>; cd Week_5`
2.  `pip install -r requirements.txt` (Python 3.9+)
3.  Install FFmpeg (see FFmpeg.org), add `bin` to PATH.
4.  Verify: `python --version; ffmpeg -version`

**Usage**

1.  `python main.py --file <npy_file> --mode <brightness|color> --output_dir <output_directory> [--downsample_factor <int>] [--max_pixels <int>]`

2.  Examples:

    -   `python main.py --file images.npy --mode brightness --output_dir output`
    -   `python main.py --file images.npy --mode color --output_dir output --downsample_factor 20 --max_pixels 5000`

**Outputs**

*   `data.csv`: Processed data.
*   `sound.wav`: Sonified output.

**Troubleshooting**

*   "FFmpeg not found": Check installation and PATH.
*   Performance: Use `--downsample_factor` or `--max_pixels`.
*   Python: Requires 3.9+.

**Updates (Developers)**

1.  `git add .`
2.  `git commit -m "Message"`
3.  `git push origin main`
4.  `git tag v1.0 && git push origin v1.0`
