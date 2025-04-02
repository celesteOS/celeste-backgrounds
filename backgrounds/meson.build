dataconf = configuration_data()
dataconf.set('BACKGROUNDDIR', backgrounddir)
dataconf.set('datadir', datadir)

backgrounds = [
  'celeste_dark.png',
  'celeste_light.png'
]

install_data(backgrounds, install_dir: backgrounddir)

foreach metadata : [
  'celeste.xml']
  configure_file(
    input: metadata + '.in',
    output: metadata,
    configuration: dataconf,
    install: true,
    install_dir: metadatadir
  )
endforeach
