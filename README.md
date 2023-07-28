# 13.3_K8S_Aleksandr_Molokov

### Задание 1. Создать Deployment приложения и решить возникшую проблему с помощью ConfigMap. Добавить веб-страницу

1. Создать Deployment приложения, состоящего из контейнеров nginx и multitool.
2. Решить возникшую проблему с помощью ConfigMap.
3. Продемонстрировать, что pod стартовал и оба конейнера работают.
4. Сделать простую веб-страницу и подключить её к Nginx с помощью ConfigMap. Подключить Service и показать вывод curl или в браузере.
5. Предоставить манифесты, а также скриншоты или вывод необходимых команд.

### Ответ

### Задания 1-3

#### ![Deployment](https://github.com/ALEMOLOKOV/13.3_K8S_Aleksandr_Molokov/blob/4d8556ca6fcef1e4437d186e400d8edda26110f0/deployment.yaml)

#### ![Configmap](https://github.com/ALEMOLOKOV/13.3_K8S_Aleksandr_Molokov/blob/4d8556ca6fcef1e4437d186e400d8edda26110f0/configmap.yaml)

#### Состояние пода

![под поднялся все работает](https://github.com/ALEMOLOKOV/13.3_K8S_Aleksandr_Molokov/assets/109212419/cae04a39-ab1a-47d5-8054-19e5b1407669)

### Задания 4-5

#### ![Deployment](https://github.com/ALEMOLOKOV/13.3_K8S_Aleksandr_Molokov/blob/4d8556ca6fcef1e4437d186e400d8edda26110f0/deploy-nginx.yaml)

#### ![Configmap](https://github.com/ALEMOLOKOV/13.3_K8S_Aleksandr_Molokov/blob/4d8556ca6fcef1e4437d186e400d8edda26110f0/nginx-conf%20configmap.yaml)

#### ![Service](https://github.com/ALEMOLOKOV/13.3_K8S_Aleksandr_Molokov/blob/4d8556ca6fcef1e4437d186e400d8edda26110f0/service%20nginx-conf.yaml)

#### Состояние 

![4 задание](https://github.com/ALEMOLOKOV/13.3_K8S_Aleksandr_Molokov/assets/109212419/26aba700-0ea9-47bc-be62-17ae86892cad)

#### Curl

![curl html](https://github.com/ALEMOLOKOV/13.3_K8S_Aleksandr_Molokov/assets/109212419/e4ff4070-f1d8-4e6c-b4e2-ab9d5bfa2fc0)



------

### Задание 2. Создать приложение с вашей веб-страницей, доступной по HTTPS 

1. Создать Deployment приложения, состоящего из Nginx.
2. Создать собственную веб-страницу и подключить её как ConfigMap к приложению.
3. Выпустить самоподписной сертификат SSL. Создать Secret для использования сертификата.
4. Создать Ingress и необходимый Service, подключить к нему SSL в вид. Продемонстировать доступ к приложению по HTTPS. 
5. Предоставить манифесты, а также скриншоты или вывод необходимых команд.


### Ответ

