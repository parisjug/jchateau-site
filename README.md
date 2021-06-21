
# Build

```bash
mvn clean site site:run
```

# Deploy sur github page

Update  `settings.xml`:

```xml
<server>
    <id>github</id>
    <password>OAUTH2TOKEN</password>
    <!-- it's password, not oauth2Token -->
</server>
```

Active profil `deploy` by running :

```bash
mvn clean site -Pdeploy
```

