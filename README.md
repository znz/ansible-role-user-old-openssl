# Ansible role for old openssl of user

- Setup old openssl into home directory

## Requirements

- Debian
- Ubuntu

## Role Variables

- `old_openssl_download_dir`: download directory
- `old_openssl_build_dir`: build directory
- `old_openssl_prefix`: prefix argument of configure
- `old_openssl_version`: openssl version
- `old_openssl_sha256`: tarball checksum of old openssl

## Dependencies

None.

## Example Playbook

Normal usage:

    ---
    - hosts: all
      become: no
      roles:
      - znz.user-old-openssl

## Example requirements.yml

    - src: https://github.com/znz/ansible-role-user-old-openssl
      version: master
      name: znz.user-old-openssl

## License

MIT License
