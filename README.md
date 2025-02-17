# This is a simple vue transition leak reproduction

Install and serve this small reproduction. You will be able to witness memory leak by clicking `Show` and `Hide` buttons. In the chrome devtools `Memory` tab you can see that each step of clicking `Show` then `Hide` button you would get additional detached elements in the snapshot. This detached elements are multiplied by number of clicking `Hide` button.
![image](https://github.com/user-attachments/assets/4b65ae5f-61f2-4f4d-918d-fc5d63404d6e)

![image](https://github.com/user-attachments/assets/67091e7d-406e-4457-a883-d2830d6b1606)


## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```
