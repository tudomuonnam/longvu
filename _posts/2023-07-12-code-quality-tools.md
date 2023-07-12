---
layout: post
title: Code Quality Testing
subtitle: Tổng hợp tool quality test cho bài code python
cover-img: 
thumbnail-img: /assets/img/code-quality.jpg
share-img: /assets/img/code-quality.jpg
tags: [test,lint,ci-cd,DevOps]
comments: true
---
> Trước giờ hay sử dụng python cho automation và viết code nho nhỏ như fastapi. Các bài code thường nhỏ nên ít sử dụng các công cụ test. Nay có hiểu biết thêm về DevOps và CI-CD thấy việc sử dụng các công cụ test là nên làm và nên sử dụng. 
>
> Bài viết này nhằm giới thiệu các công cụ test quality code (bên cạnh các bài test khác) gồm:`autoflake`,`isort`,`black` 

<figure>
<img src="/assets/img/code-quality.jpg" alt="team-work" style="border: 2px solid  gray;">
<figcaption>Code Quality là thành phần quan trọng trong môi trường Dev.  Photo by <a href="https://unsplash.com/@riku?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Riku Lu</a> on <a href="https://unsplash.com/photos/wvJuYrM5iuw?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Unsplash</a>
  </figcaption>
</figure>

## Code Quality là gì?
Code quality là quá trình đo lường, đánh giá chất lượng của code. Code chất lượng được thể hiện trên nhiều khía cạnh như:
- Tính rõ ràng: Code phải dễ đọc, dễ hiểu với tên biến, tên hàm, các comment ...
- Hiệu quả: Code chạy tốn ít tài nguyên nhất có thể
- Độ tin cậy: Code không có lỗi khi chạy, hoặc chống chịu tốt với lỗi.
- Dễ kiểm tra, bảo trì

Trong các mục trên, việc đơn giản nhất là đảm bảo code đơn giản, đúng format, dễ đọc, không khai báo thừa thư viện hay biến.

Bài viết này giới thiệu 3 công cụ đơn giản như vậy 
## 1. Isort - Sort Import
> isort là thư viện/tiện ích tự động sắp xếp các hàm import trong chương trình theo thứ tự a->z
>
Cách cài đặt 
```bash
pip install isort
```
Cách sử dụng:
```bash
isort <folder1> <folder 2> --profile black
isort src tests --profile black #sort import theo định dạng của black (xem thêm phần sau)
isort . #sort for current directory 
isort **/*.py -c -v # Check nếu file cần thay đổi sẽ in ra std
isort mypythonfile.py --diff # Xem nếu dùng isort sẽ thay đổi ra sao
```
Một vài tiện ích 
`--line-length 79`: Sẽ ngắt nếu dòng import nhiều hơn 79 kí tự (tránh code quá dài)


## 2. Autoflake

> `Autoflake` loại bỏ các hàm import và các biến khai báo **nhưng** không sử dụng trong python. Autoflake cũng loại bỏ các câu lệnh `pass` vô nghĩa trong chương trình.
Cài đặt
```bash
pip install autoflake
```
Sử dụng
Thường dùng:
```bash
autoflake --in-place --remove-unused-variables example.py
```
Đầy đủ config

```bash
usage: autoflake [-h] [-c | -cd] [-r] [-j n] [--exclude globs] [--imports IMPORTS] [--expand-star-imports] [--remove-all-unused-imports] [--ignore-init-module-imports] [--remove-duplicate-keys] [--remove-unused-variables]
                 [--remove-rhs-for-unused-variables] [--ignore-pass-statements] [--ignore-pass-after-docstring] [--version] [--quiet] [-v] [--stdin-display-name STDIN_DISPLAY_NAME] [--config CONFIG_FILE] [-i | -s]
                 files [files ...]

Removes unused imports and unused variables as reported by pyflakes.

positional arguments:
  files                 files to format

options:
  -h, --help            show this help message and exit
  -c, --check           return error code if changes are needed
  -cd, --check-diff     return error code if changes are needed, also display file diffs
  -r, --recursive       drill down directories recursively
  -j n, --jobs n        number of parallel jobs; match CPU count if value is 0 (default: 0)
  --exclude globs       exclude file/directory names that match these comma-separated globs
  --imports IMPORTS     by default, only unused standard library imports are removed; specify a comma-separated list of additional modules/packages
  --expand-star-imports
                        expand wildcard star imports with undefined names; this only triggers if there is only one star import in the file; this is skipped if there are any uses of `__all__` or `del` in the file
  --remove-all-unused-imports
                        remove all unused imports (not just those from the standard library)
  --ignore-init-module-imports
                        exclude __init__.py when removing unused imports
  --remove-duplicate-keys
                        remove all duplicate keys in objects
  --remove-unused-variables
                        remove unused variables
  --remove-rhs-for-unused-variables
                        remove RHS of statements when removing unused variables (unsafe)
  --ignore-pass-statements
                        ignore all pass statements
  --ignore-pass-after-docstring
                        ignore pass statements after a newline ending on '"""'
  --version             show program's version number and exit
  --quiet               Suppress output if there are no issues
  -v, --verbose         print more verbose logs (you can repeat `-v` to make it more verbose)
  --stdin-display-name STDIN_DISPLAY_NAME
                        the name used when processing input from stdin
  --config CONFIG_FILE  Explicitly set the config file instead of auto determining based on file location
  -i, --in-place        make changes to files instead of printing diffs
  -s, --stdout          print changed text to stdout. defaults to true when formatting stdin, or to false otherwise
```
## 3. Black - Định dạng lại code

`Black` sử dụng PEP8 để định dạng lại code python. `Black` có thể tích hợp vào trình soạn thảo code (trong file `.toml`) hoặc trong CI/CD pipeline để reformat lại source code cho dễ đọc hơn.
Cài đặt
```bash
pip install black
```
Sử dụng
```bash
black {source_file_or_directory}
```
Ví dụ
```bash
$ black --code "print ( 'hello, world' )"
print("hello, world")
```
`-l, --line-length` quy định tối đa số kí tự một dòng code có thể
Ngoài ra còn nhiều tùy chọn khác, bạn xem thêm ở phần tham khảo nhé

## Tổng kết

Trên đây là 3 câu lệnh thường được sử dụng để tự động chỉnh sửa lại code cho gọn gàng, đẹp mắt. Bạn có thể thêm vào trình soạn thảo trên máy để tự động chỉnh. DevOps cũng nên sử dụng các lệnh trên trong quá trình tích hợp code để reformat lại code trước khi chuyển sang các bước tiếp theo.

## Tham khảo
1. [https://black.readthedocs.io/en/stable/usage_and_configuration/the_basics.html](https://black.readthedocs.io/en/stable/usage_and_configuration/the_basics.html)
2. [https://pypi.org/project/autoflake/](https://pypi.org/project/autoflake/)
3. [https://pypi.org/project/isort/](https://pypi.org/project/isort/)
