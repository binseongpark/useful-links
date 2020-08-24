```sh
{
  // tasks.json 형식에 대한 설명서는 
    // https://go.microsoft.com/fwlink/?LinkId=733558의 내용을 참조하세요.
    "version": "2.0.0",
    "tasks": [
      {
        "label": "t",
        "type": "shell",
        "option": "watch",
        "problemMatcher": [
          "$tsc-watch"
        ],
        "command": "tsc ${file} && ts-node ${file}",
        "group": {
          "kind": "build",
          "isDefault": true
        }
      },
      {
        "type": "typescript",
        "tsconfig": "tsconfig.json",
        "option": "watch",
        "problemMatcher": [
          "$tsc-watch"
        ],
        "group": "build"
      }
    ]
  }
```