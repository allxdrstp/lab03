```ruby
alexandra@alexandra-virtual-machine:~$ export GITHUB_USERNAME=allxdrstp
alexandra@alexandra-virtual-machine:~$ cd ${GITHUB_USERNAME}/workspace
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace$ pushd .
~/allxdrstp/workspace ~/allxdrstp/workspace
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace$ source scripts/activate
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace$ git clone https://github.com/${GITHUB_USERNAME}/lab02.git projects/lab03
fatal: целевой путь «projects/lab03» уже существует и не является пустым каталогом.
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace$ cd projects/lab03
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ git remote remove origin
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ git remote add origin https://github.com/${GITHUB_USERNAME}/lab03.git
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ g++ -std=c++11 -I./include -c sources/print.cpp
cc1plus: fatal error: sources/print.cpp: Нет такого файла или каталога
compilation terminated.
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ g++ -std=c++11 -I./include -c sources/print.cpp
cc1plus: fatal error: sources/print.cpp: Нет такого файла или каталога
compilation terminated.
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ ^C
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ pwd
/home/alexandra/allxdrstp/workspace/projects/lab03
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ g++ -std=c++11 -I./include -c src/sources/print.cpp
cc1plus: fatal error: src/sources/print.cpp: Нет такого файла или каталога
compilation terminated.
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ ls -a sources
ls: невозможно получить доступ к 'sources': Нет такого файла или каталога
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ cd ..
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects$ cd lab02
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab02$ ls
examples  include  README.md  reports  sources  tasks
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab02$ git status
Текущая ветка: master
Неотслеживаемые файлы:
  (используйте «git add <файл>...», чтобы добавить в то, что будет включено в коммит)
	reports/
	tasks/

индекс пуст, но есть неотслеживаемые файлы
(используйте «git add», чтобы проиндексировать их)
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab02$ rm -rf tasks
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab02$ ls reports
lab02
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab02$ cat ./reports/lab02
cat: ./reports/lab02: Это каталог
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab02$ тогда rm -rf reports
тогда: команда не найдена
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab02$ rm -rf reports
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab02$ rm -rf git
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab02$ rm -rf .git
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab02$ git init -b main
Инициализирован пустой репозиторий Git в /home/alexandra/allxdrstp/workspace/projects/lab02/.git/
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab02$ git add .
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab02$ git commit -m "done"
[main (корневой коммит) bd60161] done
 5 files changed, 18 insertions(+)
 create mode 100644 README.md
 create mode 100644 examples/example1.cpp
 create mode 100644 examples/example2.cpp
 create mode 100644 include/print.hpp
 create mode 100644 sources/print.cpp
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab02$ git push origin main
fatal: 'origin' does not appear to be a git repository
fatal: Не удалось прочитать из внешнего репозитория.

Удостоверьтесь, что у вас есть необходимые права доступа
и репозиторий существует.
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab02$ git remote add origin git@github.com:allxdrstp/lab02.git
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab02$ git push origin main
To github.com:allxdrstp/lab02.git
 ! [rejected]        main -> main (fetch first)
error: не удалось отправить некоторые ссылки в «github.com:allxdrstp/lab02.git»
подсказка: Обновления были отклонены, так как внешний репозиторий содержит
подсказка: изменения, которых у вас нет в вашем локальном репозитории.
подсказка: Обычно, это связанно с тем, что кто-то уже отправил изменения в 
подсказка: то же место. Перед повторной отправкой ваших изменений, вам нужно
подсказка: забрать и слить изменения из внешнего репозитория себе
подсказка: (например, с помощью «git pull ...»).
подсказка: Для дополнительной информации, смотрите «Заметку о быстрой перемотке»
подсказка: в «git push --help».
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab02$ git push origin main --force
Перечисление объектов: 8, готово.
Подсчет объектов: 100% (8/8), готово.
При сжатии изменений используется до 4 потоков
Сжатие объектов: 100% (5/5), готово.
Запись объектов: 100% (8/8), 646 байтов | 92.00 КиБ/с, готово.
Всего 8 (изменений 0), повторно использовано 0 (изменений 0), повторно использовано пакетов 0
To github.com:allxdrstp/lab02.git
 + d317438...bd60161 main -> main (forced update)
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab02$ cd ..
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects$ rm -rf lab03
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects$ git clone git@github.com:allxdrstp/lab02.git ./lab03
Клонирование в «./lab03»...
remote: Enumerating objects: 11, done.
remote: Counting objects: 100% (11/11), done.
remote: Compressing objects: 100% (7/7), done.
remote: Total 11 (delta 1), reused 10 (delta 0), pack-reused 0
Получение объектов: 100% (11/11), готово.
Определение изменений: 100% (1/1), готово.
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects$ cd lab03
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ git remote remove origin
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ git remote add origin git@github.com:allxdrstp/lab03.git
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ g++ -std=c++11 -I./include -c sources/print.cpp
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ ls print.o
print.o
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ nm print.o 
                 U __cxa_atexit
                 U __dso_handle
                 U _GLOBAL_OFFSET_TABLE_
00000000000000aa t _GLOBAL__sub_I__Z5printRKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEERSo
0000000000000054 t _Z41__static_initialization_and_destruction_0ii
0000000000000000 T _Z5printRKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEERSo
000000000000002a T _Z5printRKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEERSt14basic_ofstreamIcS2_E
                 U _ZNSt8ios_base4InitC1Ev
                 U _ZNSt8ios_base4InitD1Ev
0000000000000000 r _ZStL19piecewise_construct
0000000000000000 b _ZStL8__ioinit
                 U _ZStlsIcSt11char_traitsIcESaIcEERSt13basic_ostreamIT_T0_ES7_RKNSt7__cxx1112basic_stringIS4_S5_T1_EE
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ ar rvs print.a print.o
ar: создаётся print.a
a - print.o
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ file print.a
print.a: current ar archive
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ g++ -std=c++11 -I./include -c examples/example1.cpp
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ ls example1.o
example1.o
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ g++ example1.o print.a -o example1
/usr/bin/ld: /usr/lib/gcc/x86_64-linux-gnu/11/../../../x86_64-linux-gnu/Scrt1.o: в функции «_start»:
(.text+0x1b): неопределённая ссылка на «main»
collect2: error: ld returned 1 exit status
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ ./example1 && echo
bash: ./example1: Нет такого файла или каталога
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ cat example1
cat: example1: Нет такого файла или каталога
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ cat examples/example1.cpp
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ g++ example1.o print.a -o example1
/usr/bin/ld: /usr/lib/gcc/x86_64-linux-gnu/11/../../../x86_64-linux-gnu/Scrt1.o: в функции «_start»:
(.text+0x1b): неопределённая ссылка на «main»
collect2: error: ld returned 1 exit status
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ cat > examples/example1.cpp <<EOF
> #include <print.hpp>

int main(int argc, char** argv)
{
  print("hello");
}
EOF
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ cat > examples/example2.cpp <<EOF
> #include <print.hpp>

#include <fstream>

int main(int argc, char** argv)
{
  std::ofstream file("log.txt");
  print(std::string("hello"), file);
}
EOF
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ g++ example1.o print.a -o example1
/usr/bin/ld: /usr/lib/gcc/x86_64-linux-gnu/11/../../../x86_64-linux-gnu/Scrt1.o: в функции «_start»:
(.text+0x1b): неопределённая ссылка на «main»
collect2: error: ld returned 1 exit status
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ g++ -std=c++11 -I./include -c examples/example1.cpp
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ ls example1.o
example1.o
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ g++ example1.o print.a -o example1
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ ./example1 && echo
hello
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ g++ -std=c++11 -I./include -c examples/example2.cpp
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ nm example2.o
                 U __cxa_atexit
                 U __dso_handle
0000000000000000 V DW.ref.__gxx_personality_v0
                 U _GLOBAL_OFFSET_TABLE_
000000000000017e t _GLOBAL__sub_I_main
                 U __gxx_personality_v0
0000000000000000 T main
                 U __stack_chk_fail
                 U _Unwind_Resume
0000000000000128 t _Z41__static_initialization_and_destruction_0ii
                 U _Z5printRKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEERSt14basic_ofstreamIcS2_E
                 U _ZNSaIcEC1Ev
                 U _ZNSaIcED1Ev
                 U _ZNSt14basic_ofstreamIcSt11char_traitsIcEEC1EPKcSt13_Ios_Openmode
                 U _ZNSt14basic_ofstreamIcSt11char_traitsIcEED1Ev
                 U _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEC1EPKcRKS3_
                 U _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEED1Ev
                 U _ZNSt8ios_base4InitC1Ev
                 U _ZNSt8ios_base4InitD1Ev
0000000000000000 r _ZStL19piecewise_construct
0000000000000000 b _ZStL8__ioinit
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ g++ example2.o print.a -o example2
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ ./example2
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ cat log.txt && echo
hello
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ rm -rf example1.o example2.o print.o
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ rm -rf print.a
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ rm -rf example1 example2
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ rm -rf log.txt


alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ \cat > CMakeLists.txt <<EOF
> cmake_minimum_required(VERSION 3.4)
project(print)
EOF
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ cat >> CMakeLists.txt <<EOF
> set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
EOF
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ cat >> CMakeLists.txt <<EOF
> add_library(print STATIC \${CMAKE_CURRENT_SOURCE_DIR}/sources/print.cpp)
EOF
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ cat >> CMakeLists.txt <<EOF
> include_directories(\${CMAKE_CURRENT_SOURCE_DIR}/include)
EOF
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ cmake -H. -B_build
-- Configuring done
-- Generating done
-- Build files have been written to: /home/alexandra/allxdrstp/workspace/projects/lab03/_build
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ cmake --build _build
Consolidate compiler generated dependencies of target print
[100%] Built target print
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ cat >> CMakeLists.txt <<EOF
> add_executable(example1 \${CMAKE_CURRENT_SOURCE_DIR}/examples/example1.cpp)
add_executable(example2 \${CMAKE_CURRENT_SOURCE_DIR}/examples/example2.cpp)
EOF
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ cat >> CMakeLists.txt <<EOF
> target_link_libraries(example1 print)
target_link_libraries(example2 print)
EOF
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ cmake --build _build
-- Configuring done
-- Generating done
-- Build files have been written to: /home/alexandra/allxdrstp/workspace/projects/lab03/_build
Consolidate compiler generated dependencies of target print
[ 33%] Built target print
Consolidate compiler generated dependencies of target example1
[ 66%] Built target example1
Consolidate compiler generated dependencies of target example2
[100%] Built target example2
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ cmake --build _build --target print
[100%] Built target print
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ cmake --build _build --target example1
[ 50%] Built target print
[100%] Built target example1
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ cmake --build _build --target example2
[ 50%] Built target print
[100%] Built target example2
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ ls -la _build/libprint.a
-rw-rw-r-- 1 alexandra alexandra 3126 мая 19 16:54 _build/libprint.a
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ _build/example1 && echo
hello
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ _build/example2
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ cat log.txt && echo
hello
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ rm -rf log.txt
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ git clone https://github.com/tp-labs/lab03 tmp
Клонирование в «tmp»...
remote: Enumerating objects: 91, done.
remote: Counting objects: 100% (30/30), done.
remote: Compressing objects: 100% (9/9), done.
remote: Total 91 (delta 23), reused 21 (delta 21), pack-reused 61
Получение объектов: 100% (91/91), 1.02 МиБ | 3.60 МиБ/с, готово.
Определение изменений: 100% (41/41), готово.
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ mv -f tmp/CMakeLists.txt .
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ rm -rf tmp
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ cat CMakeLists.txt
cmake_minimum_required(VERSION 3.4)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

option(BUILD_EXAMPLES "Build examples" OFF)

project(print)

add_library(print STATIC ${CMAKE_CURRENT_SOURCE_DIR}/sources/print.cpp)

target_include_directories(print PUBLIC
  $<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}/include>
  $<INSTALL_INTERFACE:include>
)

if(BUILD_EXAMPLES)
  file(GLOB EXAMPLE_SOURCES "${CMAKE_CURRENT_SOURCE_DIR}/examples/*.cpp")
  foreach(EXAMPLE_SOURCE ${EXAMPLE_SOURCES})
    get_filename_component(EXAMPLE_NAME ${EXAMPLE_SOURCE} NAME_WE)
    add_executable(${EXAMPLE_NAME} ${EXAMPLE_SOURCE})
    target_link_libraries(${EXAMPLE_NAME} print)
    install(TARGETS ${EXAMPLE_NAME}
      RUNTIME DESTINATION bin
    )
  endforeach(EXAMPLE_SOURCE ${EXAMPLE_SOURCES})
endif()

install(TARGETS print
    EXPORT print-config
    ARCHIVE DESTINATION lib
    LIBRARY DESTINATION lib
)

install(DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}/include/ DESTINATION include)
install(EXPORT print-config DESTINATION cmake)
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ cmake -H. -B_build -DCMAKE_INSTALL_PREFIX=_install
-- Configuring done
-- Generating done
-- Build files have been written to: /home/alexandra/allxdrstp/workspace/projects/lab03/_build
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ cmake --build _build --target install
Consolidate compiler generated dependencies of target print
[100%] Built target print
Install the project...
-- Install configuration: ""
-- Installing: /home/alexandra/allxdrstp/workspace/projects/lab03/_install/lib/libprint.a
-- Installing: /home/alexandra/allxdrstp/workspace/projects/lab03/_install/include
-- Installing: /home/alexandra/allxdrstp/workspace/projects/lab03/_install/include/print.hpp
-- Installing: /home/alexandra/allxdrstp/workspace/projects/lab03/_install/cmake/print-config.cmake
-- Installing: /home/alexandra/allxdrstp/workspace/projects/lab03/_install/cmake/print-config-noconfig.cmake
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ tree _install
_install
├── cmake
│   ├── print-config.cmake
│   └── print-config-noconfig.cmake
├── include
│   └── print.hpp
└── lib
    └── libprint.a

3 directories, 4 files
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ git add CMakeLists.txt
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ git commit -m"added CMakeLists.txt"
[main 6f51054] added CMakeLists.txt
 1 file changed, 36 insertions(+)
 create mode 100644 CMakeLists.txt
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ git push origin main
To github.com:allxdrstp/lab03.git
 ! [rejected]        main -> main (fetch first)
error: не удалось отправить некоторые ссылки в «github.com:allxdrstp/lab03.git»
подсказка: Обновления были отклонены, так как внешний репозиторий содержит
подсказка: изменения, которых у вас нет в вашем локальном репозитории.
подсказка: Обычно, это связанно с тем, что кто-то уже отправил изменения в 
подсказка: то же место. Перед повторной отправкой ваших изменений, вам нужно
подсказка: забрать и слить изменения из внешнего репозитория себе
подсказка: (например, с помощью «git pull ...»).
подсказка: Для дополнительной информации, смотрите «Заметку о быстрой перемотке»
подсказка: в «git push --help».
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ git push origin main -f
Перечисление объектов: 11, готово.
Подсчет объектов: 100% (11/11), готово.
При сжатии изменений используется до 4 потоков
Сжатие объектов: 100% (8/8), готово.
Запись объектов: 100% (11/11), 1.31 КиБ | 1.31 МиБ/с, готово.
Всего 11 (изменений 1), повторно использовано 6 (изменений 0), повторно использовано пакетов 0
remote: Resolving deltas: 100% (1/1), done.
To github.com:allxdrstp/lab03.git
 + 366b40c...6f51054 main -> main (forced update)
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ git push origin main
Everything up-to-date
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/projects/lab03$ popd
~/allxdrstp/workspace
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace$ export LAB_NUMBER=03
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace$ git clone https://github.com/tp-labs/lab${LAB_NUMBER} tasks/lab${LAB_NUMBER}
fatal: целевой путь «tasks/lab03» уже существует и не является пустым каталогом.
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace$ mkdir reports/lab${LAB_NUMBER}
mkdir: невозможно создать каталог «reports/lab03»: Файл существует
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace$ cp tasks/lab${LAB_NUMBER}/README.md reports/lab${LAB_NUMBER}/REPORT.md
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace$ cd reports/lab${LAB_NUMBER}
alexandra@alexandra-virtual-machine:~/allxdrstp/workspace/reports/lab03$ gist REPORT.md
Error: Got Net::HTTPUnauthorized from gist: {"message":"Bad credentials","documentation_url":"https://docs.github.com/rest"}
```
