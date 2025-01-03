<p align="center">
  <img src="https://raw.githubusercontent.com/0xgh057r3c0n/HelioCORS/main/logo/logo.webp" alt="Croscan Logo" width="200" style="border-radius: 10px;">
</p>

<h1 align="center">
  HelioCORS
  <br>
<sub><i>Advanced CORS Vulnerability Detection Tool</i></sub><br>
</h1>

<p align="center">
  <a href="#installation">
    <img src="https://img.shields.io/badge/installation-⚙️-blue?style=for-the-badge&logo=python" alt="Installation">
  </a> 

  <a href="#examples">
    <img src="https://img.shields.io/badge/examples-🚀-green?style=for-the-badge" alt="Examples">
  </a> 

  <a href="https://github.com/0xgh057r3c0n/HelioCORS?tab=MIT-1-ov-file" style="text-decoration: none; margin: 0 10px;">
    <img src="https://img.shields.io/badge/license-📜-red?style=for-the-badge" alt="License" style="vertical-align: middle;">
  </a>

  <a href="#usage" style="text-decoration: none; margin: 0 10px;">
    <img src="https://img.shields.io/badge/using-🛠️-purple?style=for-the-badge" alt="Using" style="vertical-align: middle;">
  </a>
</p>



## About
Corscan is a tool designed to inspect and assess Cross-Origin Resource Sharing (CORS) headers for potential vulnerabilities. It supports single URL checks and batch processing from files.
## Disclaimer
 This tool is for ethical hacking, legal, and educational use only. Any illegal use is strictly prohibited.


<h2 id="features" style="text-align: center;">🌟 Features</h2>
<ul style="text-align: center; font-size: 14px; list-style-type: none; padding: 0;">
  <li>Check and analyze CORS headers for vulnerabilities.</li>
  <li>You can run both <code>python3 heliocors.py</code> and <code>corscan</code> commands for enhanced flexibility.</li>
  <li>Customizable origin for CORS checks (default: <code>https://evil.com</code>).</li>
  <li>Bypass mechanisms for custom origin checks.</li>
  <li>Multi-threaded scanning for faster results (default: <code>20</code> threads).</li>
  <li>Output formats: <code>text</code> or <code>json</code>.</li>
  <li>Filter results to show only vulnerable entries.</li>
  <li>Save output to a specified file.</li>
</ul>


## Installation
 Clone the repository:
   ```bash
    
    git clone https://github.com/0xgh057r3c0n/HelioCORS.git
    cd HelioCORS
    python3 setup.py install

   ```
<h2 id="usage" style="text-align: center;">Usage</h2>
<p style="text-align: center; font-size: 16px;">
  <strong> python3 heliocors.py [options]</strong>
</p>
<p style="text-align: center; font-size: 14px;">
  <strong>Options:</strong><br>
  <code>-u, --url</code> Target URL to check CORS headers<br>
  <code>-f, --file</code> File containing a list of URLs to check CORS headers<br>
  <code>-r, --origin</code> Custom origin to use for the CORS check (default: <code>https://evil.com</code>)<br>
  <code>-t, --threads</code> Number of threads to use for scanning (default: <code>20</code>)<br>
  <code>-o, --output</code> File to save the output<br>
  <code>--format</code> Output format: <code>text</code> (default) or <code>json</code><br>
  <code>--filter</code> Filter results to show only vulnerable entries<br>
  <code>-h, --help</code> Show this help message and exit
</p>

## 🚀Examples

Here are some examples of how to use the Croscan Tool with the `python3 heliocors.py` command:

Check a single URL:
  ```bash
   python3 heliocors.py -u https://example.com
   ```
Check a list of URLs from a file:
```bash
python3 heliocors.py -f urls.txt
```
Use a custom origin for CORS check:

```bash
python3 heliocors.py -u https://example.com -r https://myorigin.com
```

Use multiple threads for faster scanning:
```bash
python3 heliocors.py -f urls.txt  -t 50
```
Save the output to a file:
```bash
python3 heliocors.py -f urls.txt  -o result.txt
```
Output in JSON format:
```bash
python3 heliocors.py -f urls.txt  --format json
```
Filter results to show only vulnerable entries:
```bash
python3 heliocors.py -f urls.txt --filter
```