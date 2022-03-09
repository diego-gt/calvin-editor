project(
  'calvin_editor',
  'cpp',
  version : '0.1',
  default_options : [
    'warning_level=3',
    'cpp_std=c++20'
    ])

editor_includes = include_directories('include')

editor_sources = files([
  'src/main.cpp'
  ])

imgui_proj = subproject('imgui')
imgui_dep = imgui_proj.get_variable('imgui_dep')
glfw3_dep = dependency('glfw3', version : '>=3.3')
vulkan_dep = dependency('vulkan', version : '>=1.2')

editor_exe = executable(
  'calvin_editor',
  editor_sources,
  install : false,
  include_directories : editor_includes,
  dependencies : [ imgui_dep, glfw3_dep, vulkan_dep ]
  )

