# Maintainer: Philip Müller <philm[at]manjaro[dot]org>
# Maintainer: Helmut Stult <helmut[at]manjaro[dot]org>

# Arch credits:
# Tobias Powalowski <tpowa@archlinux.org>
# Thomas Baechler <thomas@archlinux.org>

# Cloud Server
_server=cpx51

pkgbase=linux58
pkgname=('linux58' 'linux58-headers')
_kernelname=-MANJARO
_basekernel=5.8
_basever=58
_aufs=20200622
pkgver=5.8.0
pkgrel=2
arch=('x86_64')
url="http://www.kernel.org/"
license=('GPL2')
makedepends=('bc'
    'docbook-xsl'
    'elfutils'
    'git'
    'inetutils'
    'kmod'
    'xmlto')
options=('!strip')
source=("https://www.kernel.org/pub/linux/kernel/v5.x/linux-${_basekernel}.tar.xz"
        #"https://www.kernel.org/pub/linux/kernel/v5.x/patch-${pkgver}.xz"
        # the main kernel config files
        'config' 'config.aufs'
        # ARCH Patches
        '0001-ZEN-Add-sysctl-and-CONFIG-to-disallow-unprivileged-CLONE_NEWUSER.patch'
        # MANJARO Patches
        '0001-nonupstream-navi10-vfio-reset.patch'
        '0001-i2c-nuvoton-nc677x-hwmon-driver.patch'
        '0001-iomap-iomap_bmap-should-accept-unwritten-maps.patch'
        '0001-futex.patch'
        '0001-apparmor-patch-to-provide-compatibility-with-v2-net-rules.patch'
        '0002-apparmor-af_unix-mediation.patch'
        '0003-apparmor-fix-use-after-free-in-sk_peer_label.patch'
        '0004-apparmor-fix-apparmor-mediating-locking-non-fs-unix-sockets.patch'
        'virtualbox-temp.patch'

         # Lenovo + AMD
        '0001-nonupstream-navi10-vfio-reset.patch'
        '0001-lenovo-wmi2.patch'
        '0002-pinctrl-amd.patch'

        # Bootsplash
        '0001-bootsplash.patch'
        '0002-bootsplash.patch'
        '0003-bootsplash.patch'
        '0004-bootsplash.patch'
        '0005-bootsplash.patch'
        '0006-bootsplash.patch'
        '0007-bootsplash.patch'
        '0008-bootsplash.patch'
        '0009-bootsplash.patch'
        '0010-bootsplash.patch'
        '0011-bootsplash.patch'
        '0012-bootsplash.patch'
        '0013-bootsplash.patch')
sha256sums=('e7f75186aa0642114af8f19d99559937300ca27acaf7451b36d4f9b0f85cf1f5'
            '0c43d35351026c91ea92100fed692e9e43c6137bf1bef8e5c1301f56f7620a56'
            'b44d81446d8b53d5637287c30ae3eb64cae0078c3fbc45fcf1081dd6699818b5'
            '986f8d802f37b72a54256f0ab84da83cb229388d58c0b6750f7c770818a18421'
            'f1eec160ce5df5c2ea58d4e4fd44a6b1013863c6b3bf649414cd18c89ae500fa'
            '0556859a8168c8f7da9af8e2059d33216d9e5378d2cac70ca54c5ff843fa5add'
            '95745075edd597caa92b369cfbcd11a04c9e3c88c0c987c70114924e1e01df5c'
            '78dde51123a21ec5efe9c420b309d03263001dafd8684f71c167f02e3f504f9e'
            '98202b8ad70d02d86603294bae967874fa7b18704b5c7b867568b0fd33a08921'
            '5cbbf3db9ea3205e9b89fe3049bea6dd626181db0cb0dc461e4cf5a400c68dd6'
            'c7dbec875d0c1d6782c037a1dcefff2e5bdb5fc9dffac1beea07dd8c1bdef1d7'
            '77746aea71ffb06c685e7769b49c78e29af9b2e28209cd245e95d9cbb0dba3c9'
            'c98893aafd51e83107bb6823cbe3c63ee85c00f439c1facaed3b6ab3c0490e98'
            'f1eec160ce5df5c2ea58d4e4fd44a6b1013863c6b3bf649414cd18c89ae500fa'
            '1d58ef2991c625f6f0eb33b4cb8303932f53f1c4694e42bae24c9cd36d2ad013'
            '427fd41ac742110d413f01daba66d5cd023b8e63fdc63242fcc96f589e66867f'
            'a504f6cf84094e08eaa3cc5b28440261797bf4f06f04993ee46a20628ff2b53c'
            'e096b127a5208f56d368d2cb938933454d7200d70c86b763aa22c38e0ddb8717'
            '8c1c880f2caa9c7ae43281a35410203887ea8eae750fe8d360d0c8bf80fcc6e0'
            '1144d51e5eb980fceeec16004f3645ed04a60fac9e0c7cf88a15c5c1e7a4b89e'
            'dd4b69def2efacf4a6c442202ad5cb93d492c03886d7c61de87696e5a83e2846'
            '028b07f0c954f70ca37237b62e04103e81f7c658bb8bd65d7d3c2ace301297dc'
            'c8b0cb231659d33c3cfaed4b1f8d7c8305ab170bdd4c77fce85270d7b6a68000'
            '8dbb5ab3cb99e48d97d4e2f2e3df5d0de66f3721b4f7fd94a708089f53245c77'
            'a7aefeacf22c600fafd9e040a985a913643095db7272c296b77a0a651c6a140a'
            'e9f22cbb542591087d2d66dc6dc912b1434330ba3cd13d2df741d869a2c31e89'
            '27471eee564ca3149dd271b0817719b5565a9594dc4d884fe3dc51a5f03832bc'
            '60e295601e4fb33d9bf65f198c54c7eb07c0d1e91e2ad1e0dd6cd6e142cb266d'
            '035ea4b2a7621054f4560471f45336b981538a40172d8f17285910d4e0e0b3ef')
prepare() {
  cd "${srcdir}/linux-${_basekernel}"

  # add upstream patch
  #msg "add upstream patch"
  #patch -p1 -i "${srcdir}/patch-${pkgver}"

  # add latest fixes from stable queue, if needed
  # http://git.kernel.org/?p=linux/kernel/git/stable/stable-queue.git
  # enable only if you have "gen-stable-queue-patch.sh" executed before
  #patch -Np1 -i "${srcdir}/prepatch-${_basekernel}.patch"

  # disable USER_NS for non-root users by default
  msg2 "PATCH: 0001-ZEN-Add-sysctl-and-CONFIG-to-disallow-unprivileged-CLONE_NEWUSER"
  patch -Np1 -i "${srcdir}/0001-ZEN-Add-sysctl-and-CONFIG-to-disallow-unprivileged-CLONE_NEWUSER.patch"

  # other fixes by Arch

  # add patches for snapd
  # https://gitlab.com/apparmor/apparmor-kernel/tree/5.2-outoftree
  msg "add patches for snapd"
  msg2 "0001-apparmor-patch-to-provide-compatibility-with-v2-net-rules"
  patch -Np1 -i "${srcdir}/0001-apparmor-patch-to-provide-compatibility-with-v2-net-rules.patch"
  msg2 "0002-apparmor-af_unix-mediation"
  patch -Np1 -i "${srcdir}/0002-apparmor-af_unix-mediation.patch"
  msg2 "0003-apparmor-fix-use-after-free-in-sk_peer_label"
  patch -Np1 -i "${srcdir}/0003-apparmor-fix-use-after-free-in-sk_peer_label.patch"
  msg2 "0004-apparmor-fix-apparmor-mediating-locking-non-fs-unix-sockets"
  patch -Np1 -i "${srcdir}/0004-apparmor-fix-apparmor-mediating-locking-non-fs-unix-sockets.patch"

  # MANJARO Patches
  msg "nuvoton hwmon driver patch"
  # https://twitter.com/vskye11/status/1216240051639791616
  patch -Np1 -i '../0001-i2c-nuvoton-nc677x-hwmon-driver.patch'

  # Lenovo + AMD
  msg "Lenovo + AMD"

  msg2 "navi10-vfio reset patch"
  # TODO: remove when AMD properly fixes it!
  # INFO: this is a hack and won't be upstreamed
  # https://forum.level1techs.com/t/145666/86
  # https://forum.manjaro.org/t/107820/11
  patch -Np1 -i "${srcdir}/0001-nonupstream-navi10-vfio-reset.patch"

  msg2 "0001-lenovo-wmi2"
  patch -Np1 -i '../0001-lenovo-wmi2.patch'
  msg2 "0002-pinctrl-amd"
  patch -Np1 -i '../0002-pinctrl-amd.patch'

  # https://bugzilla.kernel.org/show_bug.cgi?id=207585
  msg2 "handling of multiple fans on Lenovo P50"
  patch -Np1 -i "${srcdir}/0001-iomap-iomap_bmap-should-accept-unwritten-maps.patch"

  # temp patch for VirtualBox 6.1.12
  msg2 "virtualbox-temp.patch"
  patch -Np1 -i "${srcdir}/virtualbox-temp.patch"

  # futex patch, https://lore.kernel.org/lkml/20200612185122.327860-1-andrealmeid@collabora.com/
  msg2 "0001-futex.patch"
  patch -Np1 -i "${srcdir}/0001-futex.patch"

  # Add bootsplash - http://lkml.iu.edu/hypermail/linux/kernel/1710.3/01542.html
  msg "Add bootsplash"
  msg2 "0001-bootsplash."
  patch -Np1 -i "${srcdir}/0001-bootsplash.patch"
  msg2 "0002-bootsplash"
  patch -Np1 -i "${srcdir}/0002-bootsplash.patch"
  msg2 "0003-bootsplash"
  patch -Np1 -i "${srcdir}/0003-bootsplash.patch"
  msg2 "0004-bootsplash"
  patch -Np1 -i "${srcdir}/0004-bootsplash.patch"
  msg2 "0005-bootsplash"
  patch -Np1 -i "${srcdir}/0005-bootsplash.patch"
  msg2 "0006-bootsplash"
  patch -Np1 -i "${srcdir}/0006-bootsplash.patch"
  msg2 "0007-bootsplash"
  patch -Np1 -i "${srcdir}/0007-bootsplash.patch"
  msg2 "0008-bootsplash"
  patch -Np1 -i "${srcdir}/0008-bootsplash.patch"
  msg2 "0009-bootsplash"
  patch -Np1 -i "${srcdir}/0009-bootsplash.patch"
  msg2 "0010-bootsplash."
  patch -Np1 -i "${srcdir}/0010-bootsplash.patch"
  msg2 "0011-bootsplash"
  patch -Np1 -i "${srcdir}/0011-bootsplash.patch"
  msg2 "0012-bootsplash"
  patch -Np1 -i "${srcdir}/0012-bootsplash.patch"
  # use git-apply to add binary files
  msg2 "0013-bootsplash"
  git apply -p1 < "${srcdir}/0013-bootsplash.patch"

  cat "${srcdir}/config" > ./.config

  if [ "${_kernelname}" != "" ]; then
    sed -i "s|CONFIG_LOCALVERSION=.*|CONFIG_LOCALVERSION=\"${_kernelname}\"|g" ./.config
    sed -i "s|CONFIG_LOCALVERSION_AUTO=.*|CONFIG_LOCALVERSION_AUTO=n|" ./.config
  fi

  msg "set extraversion to pkgrel"
  sed -ri "s|^(EXTRAVERSION =).*|\1 -${pkgrel}|" Makefile

  msg "don't run depmod on 'make install'"
  # We'll do this ourselves in packaging
  sed -i '2iexit 0' scripts/depmod.sh

  msg "get kernel version"
  make prepare

  # load configuration
  # Configure the kernel. Replace the line below with one of your choice.
  #make menuconfig # CLI menu for configuration
  #make nconfig # new CLI menu for configuration
  #make xconfig # X-based configuration
  #make oldconfig # using old config from previous kernel version
  # ... or manually edit .config

  msg "rewrite configuration"
  yes "" | make config >/dev/null
}

build() {
  cd "${srcdir}/linux-${_basekernel}"

  msg "build"
  make ${MAKEFLAGS} LOCALVERSION= bzImage modules
}

package_linux58() {
  pkgdesc="The ${pkgbase/linux/Linux} kernel and modules"
  depends=('coreutils' 'linux-firmware' 'kmod' 'mkinitcpio>=27')
  optdepends=('crda: to set the correct wireless channels of your country')
  provides=("linux=${pkgver}" VIRTUALBOX-GUEST-MODULES WIREGUARD-MODULE)

  cd "${srcdir}/linux-${_basekernel}"

  KARCH=x86

  # get kernel version
  _kernver="$(make LOCALVERSION= kernelrelease)"

  mkdir -p "${pkgdir}"/{boot,usr/lib/modules}
  make LOCALVERSION= INSTALL_MOD_PATH="${pkgdir}/usr" INSTALL_MOD_STRIP=1 modules_install

  # systemd expects to find the kernel here to allow hibernation
  # https://github.com/systemd/systemd/commit/edda44605f06a41fb86b7ab8128dcf99161d2344
  cp arch/$KARCH/boot/bzImage "${pkgdir}/usr/lib/modules/${_kernver}/vmlinuz"

  # Used by mkinitcpio to name the kernel
  echo "${pkgbase}" | install -Dm644 /dev/stdin "${pkgdir}/usr/lib/modules/${_kernver}/pkgbase"
  echo "${_basekernel}-${CARCH}" | install -Dm644 /dev/stdin "${pkgdir}/usr/lib/modules/${_kernver}/kernelbase"

  # add kernel version
  echo "${pkgver}-${pkgrel}-MANJARO x64" > "${pkgdir}/boot/${pkgbase}-${CARCH}.kver"

  # make room for external modules
  local _extramodules="extramodules-${_basekernel}${_kernelname:--MANJARO}"
  ln -s "../${_extramodules}" "${pkgdir}/usr/lib/modules/${_kernver}/extramodules"

  # add real version for building modules and running depmod from hook
  echo "${_kernver}" |
    install -Dm644 /dev/stdin "${pkgdir}/usr/lib/modules/${_extramodules}/version"

  # remove build and source links
  rm "${pkgdir}"/usr/lib/modules/${_kernver}/{source,build}

  # now we call depmod...
  depmod -b "${pkgdir}/usr" -F System.map "${_kernver}"

  # add vmlinux
  install -Dt "${pkgdir}/usr/lib/modules/${_kernver}/build" -m644 vmlinux
}

package_linux58-headers() {
  pkgdesc="Header files and scripts for building modules for ${pkgbase/linux/Linux} kernel"
  provides=("linux-headers=$pkgver")

  cd "${srcdir}/linux-${_basekernel}"
  local _builddir="${pkgdir}/usr/lib/modules/${_kernver}/build"

  install -Dt "${_builddir}" -m644 Makefile .config Module.symvers
  install -Dt "${_builddir}/kernel" -m644 kernel/Makefile

  mkdir "${_builddir}/.tmp_versions"

  cp -t "${_builddir}" -a include scripts

  install -Dt "${_builddir}/arch/${KARCH}" -m644 "arch/${KARCH}/Makefile"
  install -Dt "${_builddir}/arch/${KARCH}/kernel" -m644 "arch/${KARCH}/kernel/asm-offsets.s"
  #install -Dt "${_builddir}/arch/${KARCH}/kernel" -m644 "arch/${KARCH}/kernel/macros.s"

  cp -t "${_builddir}/arch/${KARCH}" -a "arch/${KARCH}/include"

  install -Dt "${_builddir}/drivers/md" -m644 drivers/md/*.h
  install -Dt "${_builddir}/net/mac80211" -m644 net/mac80211/*.h

  # http://bugs.archlinux.org/task/13146
  install -Dt "${_builddir}/drivers/media/i2c" -m644 drivers/media/i2c/msp3400-driver.h

  # http://bugs.archlinux.org/task/20402
  install -Dt "${_builddir}/drivers/media/usb/dvb-usb" -m644 drivers/media/usb/dvb-usb/*.h
  install -Dt "${_builddir}/drivers/media/dvb-frontends" -m644 drivers/media/dvb-frontends/*.h
  install -Dt "${_builddir}/drivers/media/tuners" -m644 drivers/media/tuners/*.h

  # add xfs and shmem for aufs building
  mkdir -p "${_builddir}"/{fs/xfs,mm}

  # copy in Kconfig files
  find . -name Kconfig\* -exec install -Dm644 {} "${_builddir}/{}" \;

  # add objtool for external module building and enabled VALIDATION_STACK option
  install -Dt "${_builddir}/tools/objtool" tools/objtool/objtool

  # remove unneeded architectures
  local _arch
  for _arch in "${_builddir}"/arch/*/; do
    [[ ${_arch} == */x86/ ]] && continue
    rm -r "${_arch}"
  done

  # remove files already in linux-docs package
  rm -r "${_builddir}/Documentation"

  # Fix permissions
  chmod -R u=rwX,go=rX "${_builddir}"

  # strip scripts directory
  local _binary _strip
  while read -rd '' _binary; do
    case "$(file -bi "${_binary}")" in
      *application/x-sharedlib*)  _strip="${STRIP_SHARED}"   ;; # Libraries (.so)
      *application/x-archive*)    _strip="${STRIP_STATIC}"   ;; # Libraries (.a)
      *application/x-executable*) _strip="${STRIP_BINARIES}" ;; # Binaries
      *) continue ;;
    esac
    /usr/bin/strip ${_strip} "${_binary}"
  done < <(find "${_builddir}/scripts" -type f -perm -u+w -print0 2>/dev/null)
}
