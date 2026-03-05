# Netboot
Instalar uma distro Linux Ubuntu 24.04 e criar um chroot + PXE + NFS + OverlayFS + AnduinOS UI + Wine (app windows), para ficar bem parecido com o windows e boot remoto

Visão geral da arquitetura (o que vai acontecer):
- O PC cliente liga
- Pede IP via DHCP
- Recebe instrução de boot PXE
- Baixa kernel + initrd via TFTP
- Monta o sistema raiz via NFS
- O Linux roda 100% pela rede (sem HD)
