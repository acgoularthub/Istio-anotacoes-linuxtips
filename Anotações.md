# Instalação do Istio:

Com o kubectl apontando para seu cluster, vamos instalar o Istio, começando pelo download:

```bash
curl -L https://istio.io/downloadIstio | sh -
```
 (método de instalação baseado no linux, para meu caso, para mais métodos, conferir na [página do Istio](https://istio.io/latest/docs/setup/getting-started/#download))

Em seguida podemos adicionar ou cliente do Istio ao nosso `PATH` ou:

```bash
sudo cp -r istio-1.13.4/bin/istioctl /usr/local/bin/
```

Para instalar, propriamente, basta executar o comando:

```bash
istioctl install --set profile=demo -y
```

Existem diversos profiles para configurar o Istio, cada profile pode ser utilizado conforme a necessidade e podemos checar todos os profiles disponíveis na documentação oficial do Istio.

