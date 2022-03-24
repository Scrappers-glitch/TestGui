testgui_sources = [
  'main.c',
  'testgui-window.c',
]

testgui_deps = [
  dependency('gio-2.0', version: '>= 2.50'),
  dependency('gtk+-3.0', version: '>= 3.22'),
]

gnome = import('gnome')

testgui_sources += gnome.compile_resources('testgui-resources',
  'testgui.gresource.xml',
  c_name: 'testgui'
)

executable('testgui', testgui_sources,
  dependencies: testgui_deps,
  install: true,
)
