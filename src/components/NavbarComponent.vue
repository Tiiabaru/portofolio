<script setup>
import { Navbar, NavbarLogo, NavbarCollapse, NavbarLink } from 'flowbite-vue'
</script>
<template>
    <Navbar>
      <template #logo>
        <NavbarLogo link="https://www.google.com/" alt="Flowbite logo" image-url="pr.jpeg">
          TIA'WEB
        </NavbarLogo>
      </template>
      <template #default="{isShowMenu}">
        <NavbarCollapse :isShowMenu="isShowMenu">
          <NavbarLink isActive link="#">Home</NavbarLink>
          <NavbarLink link="#">Tentang</NavbarLink>
          <NavbarLink link="#">Pengalaman</NavbarLink>
          <NavbarLink link="#">Riwayat</NavbarLink>
          <NavbarLink link="#">Contact</NavbarLink>
        </NavbarCollapse>
      </template>
    </Navbar>
</template>
