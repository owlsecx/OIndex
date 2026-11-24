# Third-Party Notices — OIndex

This tool is distributed as a single pre-built executable. It bundles the
third-party components listed below. Each component remains the property of
its respective copyright holders and is used under its own license, whose
full text is reproduced in this file.

**Owlsec LLC's own source code is proprietary and is not covered by any of
the licenses below.** Those licenses apply only to the third-party components
named here.

- Tool binary: `OIndex`
- SHA-256: `6027f2a97aa1be3c332a969fd0e4ed7d28aa9a6bb79e0e5b07ebc101c5abff04`
- Bundled interpreter: CPython 3.11 (PSF License)
- Generated: 2026-11-24
- Machine-readable inventory: see `SBOM.cdx.json` in this repository

## Components

| Component | Version | License |
|---|---|---|
| googlesearch_python | 1.3.0 | MIT License |
| pyperclip | 1.11.0 | BSD |
| CPython | 3.11 | PSF-2.0 |
| Python standard library | 3.11 | PSF-2.0 |

Shared system libraries from Debian (for example `libssl`, `libz`, `libbz2`) are bundled unmodified by PyInstaller and are governed by their own licenses as shipped by the Debian project. The exact versions are listed in `SBOM.cdx.json`.

---

## Full license texts

### googlesearch_python 1.3.0

- Author: Nishant Vikramaditya
- Project: https://github.com/Nv7-GitHub/googlesearch
- Declared license: MIT License

<details>
<summary><code>LICENSE</code></summary>

```text
MIT License

Copyright (c) 2020 Nv7

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

</details>

### pyperclip 1.11.0

- Project: https://github.com/asweigart/pyperclip
- Declared license: BSD

<details>
<summary><code>LICENSE.txt</code></summary>

```text
Copyright (c) 2014, Al Sweigart
All rights reserved.

Redistribution and use in source and binary forms, with or without
modification, are permitted provided that the following conditions are met:

* Redistributions of source code must retain the above copyright notice, this
  list of conditions and the following disclaimer.

* Redistributions in binary form must reproduce the above copyright notice,
  this list of conditions and the following disclaimer in the documentation
  and/or other materials provided with the distribution.

* Neither the name of the {organization} nor the names of its
  contributors may be used to endorse or promote products derived from
  this software without specific prior written permission.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

</details>

---

## Python Software Foundation License

The bundled CPython interpreter and standard library are distributed under the PSF License Agreement: <https://docs.python.org/3/license.html>
