# Belajar Kubernetes

Ini adalah source code untuk materi screencast :

https://www.youtube.com/playlist?list=PL-CtdCApEFH8XrWyQAyRd6d_CKwxD8Ime

Anda bisa melihat slide materinya disini :

https://docs.google.com/presentation/d/1NJQqJd89k1od_o9Kz-79IQ_CQYDCJKWunCtpgkHQLi4/edit?usp=sharing

## My Curated Questions

Pertanyaan"ku yg dikurasi:

### Gimana klo mo connect docker ke private registry?

Lihat di https://kubernetes.io/docs/tasks/configure-pod-container/pull-image-private-registry/

### Gimana Cara Buat config atau secret dari file?

```sh
# cm adalah configmaps
kubectl create cm game-api --from-env-file game.properties --from-env-file ui.properties
kubectl create cm game-api --from-file game.properties --from-file ui.properties
```
