## Expected Behavior
<!--- Tell us what should happen.  What were you doing?  What part of dlib are you using?  What do you think should happen? -->
On installing dlib for python.
According to dlib.net, to install dlib for python just type "pip install dlib" or "python setup.py install" after downloading the project from github. However, in both cases, the installation has an error and does not complete.

## Current Behavior
<!--- Tell us what happens instead of the expected behavior.  If you get an error, include the entire error message in the bug report.  DO NOT POST SCREEN SHOTS.  Paste in the text instead.   If the issue is some kind of build problem, include the entire CMake output along with the error message. -->
(venv) D:\projetos\testeDlib\dlib-19.19>python setup.py install
running install
running bdist_egg
running egg_info
creating dlib.egg-info
writing dlib.egg-info\PKG-INFO
writing dependency_links to dlib.egg-info\dependency_links.txt
writing top-level names to dlib.egg-info\top_level.txt
writing manifest file 'dlib.egg-info\SOURCES.txt'
package init file 'dlib\__init__.py' not found (or not a regular file)
reading manifest file 'dlib.egg-info\SOURCES.txt'
reading manifest template 'MANIFEST.in'
no previously-included directories found matching 'tools\python\build*'
writing manifest file 'dlib.egg-info\SOURCES.txt'
installing library code to build\bdist.win-amd64\egg
running install_lib
running build_py
running build_ext
Building extension for Python 3.7.7 (tags/v3.7.7:d7c567b08f, Mar 10 2020, 10:41:24) [MSC v.1900 64 bit (AMD64)]
Invoking CMake setup: 'cmake D:\projetos\testeDlib\dlib-19.19\tools\python -DCMAKE_LIBRARY_OUTPUT_DIRECTORY=D:\projetos\testeDlib\dlib-19.19\build\lib.win-amd64-3.7 -DPYTHON_EXECUTABLE=D:\projetos\testeDlib\v
env\Scripts\python.exe -DCMAKE_LIBRARY_OUTPUT_DIRECTORY_RELEASE=D:\projetos\testeDlib\dlib-19.19\build\lib.win-amd64-3.7 -A x64'
-- Building for: Visual Studio 15 2017
CMake Error at CMakeLists.txt:3 (project):
  Failed to run MSBuild command:

    C:/Program Files (x86)/Microsoft Visual Studio/2017/Community/MSBuild/15.0/Bin/MSBuild.exe

  to get the value of VCTargetsPath:

    Microsoft(R) Build Engine versão 15.1.550.39093
    Copyright (C) Microsoft Corporation. Todos os direitos reservados.

    Compilação de 25/03/2020 22:53:10 iniciada.
    Projeto "D:\projetos\testeDlib\dlib-19.19\build\temp.win-amd64-3.7\Release\CMakeFiles\3.16.0\VCTargetsPath.vcxproj" no nó 1 (destinos padrão).
    D:\projetos\testeDlib\dlib-19.19\build\temp.win-amd64-3.7\Release\CMakeFiles\3.16.0\VCTargetsPath.vcxproj(14,2): error MSB4019: O projeto "C:\Program Files (x86)\Microsoft Visual Studio\2017\Community\Com
mon7\IDE\VC\VCTargets\Microsoft.Cpp.Default.props" importado não foi encontrado. Confirme se o caminho na declaração <Import> está correto e se o arquivo existe no disco.
    Projeto de compilação pronto "D:\projetos\testeDlib\dlib-19.19\build\temp.win-amd64-3.7\Release\CMakeFiles\3.16.0\VCTargetsPath.vcxproj" (destinos padrão) -- FALHA.

    FALHA da compilação.

    "D:\projetos\testeDlib\dlib-19.19\build\temp.win-amd64-3.7\Release\CMakeFiles\3.16.0\VCTargetsPath.vcxproj" (destino padrão) (1) ->
      D:\projetos\testeDlib\dlib-19.19\build\temp.win-amd64-3.7\Release\CMakeFiles\3.16.0\VCTargetsPath.vcxproj(14,2): error MSB4019: O projeto "C:\Program Files (x86)\Microsoft Visual Studio\2017\Community\C
ommon7\IDE\VC\VCTargets\Microsoft.Cpp.Default.props" importado não foi encontrado. Confirme se o caminho na declaração <Import> está correto e se o arquivo existe no disco.

        0 Aviso(s)
        1 Erro(s)

    Tempo Decorrido 00:00:00.04


  Exit code: 1



-- Configuring incomplete, errors occurred!
See also "D:/projetos/testeDlib/dlib-19.19/build/temp.win-amd64-3.7/Release/CMakeFiles/CMakeOutput.log".
Traceback (most recent call last):
  File "setup.py", line 261, in <module>
    'Topic :: Software Development',
  File "D:\projetos\testeDlib\venv\lib\site-packages\setuptools-40.8.0-py3.7.egg\setuptools\__init__.py", line 145, in setup
  File "C:\Users\igor\AppData\Local\Programs\Python\Python37\lib\distutils\core.py", line 148, in setup
    dist.run_commands()
  File "C:\Users\igor\AppData\Local\Programs\Python\Python37\lib\distutils\dist.py", line 966, in run_commands
    self.run_command(cmd)
  File "C:\Users\igor\AppData\Local\Programs\Python\Python37\lib\distutils\dist.py", line 985, in run_command
    cmd_obj.run()
  File "D:\projetos\testeDlib\venv\lib\site-packages\setuptools-40.8.0-py3.7.egg\setuptools\command\install.py", line 67, in run
  File "D:\projetos\testeDlib\venv\lib\site-packages\setuptools-40.8.0-py3.7.egg\setuptools\command\install.py", line 109, in do_egg_install
  File "C:\Users\igor\AppData\Local\Programs\Python\Python37\lib\distutils\cmd.py", line 313, in run_command
    self.distribution.run_command(command)
  File "C:\Users\igor\AppData\Local\Programs\Python\Python37\lib\distutils\dist.py", line 985, in run_command
    cmd_obj.run()
  File "D:\projetos\testeDlib\venv\lib\site-packages\setuptools-40.8.0-py3.7.egg\setuptools\command\bdist_egg.py", line 172, in run
  File "D:\projetos\testeDlib\venv\lib\site-packages\setuptools-40.8.0-py3.7.egg\setuptools\command\bdist_egg.py", line 158, in call_command
  File "C:\Users\igor\AppData\Local\Programs\Python\Python37\lib\distutils\cmd.py", line 313, in run_command
    self.distribution.run_command(command)
  File "C:\Users\igor\AppData\Local\Programs\Python\Python37\lib\distutils\dist.py", line 985, in run_command
    cmd_obj.run()
  File "D:\projetos\testeDlib\venv\lib\site-packages\setuptools-40.8.0-py3.7.egg\setuptools\command\install_lib.py", line 11, in run
  File "C:\Users\igor\AppData\Local\Programs\Python\Python37\lib\distutils\command\install_lib.py", line 107, in build
    self.run_command('build_ext')
  File "C:\Users\igor\AppData\Local\Programs\Python\Python37\lib\distutils\cmd.py", line 313, in run_command
    self.distribution.run_command(command)
  File "C:\Users\igor\AppData\Local\Programs\Python\Python37\lib\distutils\dist.py", line 985, in run_command
    cmd_obj.run()
  File "setup.py", line 135, in run
    self.build_extension(ext)
  File "setup.py", line 172, in build_extension
    subprocess.check_call(cmake_setup, cwd=build_folder)
  File "C:\Users\igor\AppData\Local\Programs\Python\Python37\lib\subprocess.py", line 363, in check_call
    raise CalledProcessError(retcode, cmd)
subprocess.CalledProcessError: Command '['cmake', 'D:\\projetos\\testeDlib\\dlib-19.19\\tools\\python', '-DCMAKE_LIBRARY_OUTPUT_DIRECTORY=D:\\projetos\\testeDlib\\dlib-19.19\\build\\lib.win-amd64-3.7', '-DPYT
HON_EXECUTABLE=D:\\projetos\\testeDlib\\venv\\Scripts\\python.exe', '-DCMAKE_LIBRARY_OUTPUT_DIRECTORY_RELEASE=D:\\projetos\\testeDlib\\dlib-19.19\\build\\lib.win-amd64-3.7', '-A', 'x64']' returned non-zero ex
it status 1.


## Steps to Reproduce
<!--- Provide an unambiguous set of steps to reproduce this problem.  What exactly do I have to type to reproduce your error?  If you don't post complete instructions you are much less likely to get help. -->
pip install dlib


* **Version**: <!-- What version of dlib? -->
dlib 19.19
* **Where did you get dlib**: <!-- Did you get it from an official source like dlib.net, this github repo, or somewhere else? -->
From an official source dlib.net and this github

* **Platform**: <!-- include something like `lsb_release -a` output, or if Windows, version and 32-bit or
  64-bit -->
  On windows 7, 64 bit, and linux mint, 64 bits.

* **Compiler**: <!-- What compiler are you using?  What version of that compiler? -->
Visual studio 2017, Mingw and cmake 3.16 on windows.
On Linux Mint, standard Cmake and gcc compiler.
