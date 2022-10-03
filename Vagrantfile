vagrant.configure('2') do |config|
    config.vm.box = 'ubuntu/xenial64'
    config.disksize.size = '60GB'
    config.vm.network "public_network", bridge: [
  "en0: Wi-Fi (AirPort)",
  "en6: Broadcom NetXtreme Gigabit Ethernet Controller",
]
end