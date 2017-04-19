# Работа с xen-снепшотами


### Получение списка виртаульных машин
```bash
xe vm-list
```

### Создание снепшота
```bash
xe vm-snapshot uuid=e6d067a7-5daf-47cc-a057-7b3af99ef82f new-name-label=search
```

### Экспорт в файл
```bash
xe vm-export vm=08a0cd8f-ea1f-751e-8814-82040926ff21 filename=/newstorage/search.xva
```

### Импорт из файла
```bash
xe vm-import filename=/xenbackup/search.xva
```