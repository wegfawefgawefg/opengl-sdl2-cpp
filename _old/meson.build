project('smonky', 'c',
    default_options: 'default_library=static')

cc = meson.get_compiler('cpps')
m_dep = cc.find_library('m', required : false)

sdl2_dep = dependency('sdl2')
sdl2_ttf_dep = dependency('SDL2_ttf')
sdl2_image_dep = dependency('SDL2_image')
cglm_dep = dependency('cglm')

executable( 'smonky',
    sources: [
        'main.c',
    ],
    dependencies: [
        sdl2_dep, 
        sdl2_ttf_dep, 
        sdl2_image_dep,
        cglm_dep,
        m_dep,
    ],
)
