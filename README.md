
Start Docker
```
cd pixorama_server
docker compose -p pixorama up --build --detach
```

Run Migrations
```
dart bin/main.dart --apply-migrations
```

Start Server
```
dart bin/main.dart
```

Run Flutter App (In another terminal tab)
```
cd ../pixorama_flutter
flutter run -d chrome 
```