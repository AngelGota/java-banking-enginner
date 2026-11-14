# Referencia BIAN del Proyecto 1

Versión de referencia obligatoria: **BIAN 14.0.0**.

- SD: Party Reference Data Directory.
- CR: PartyReferenceDataDirectoryEntry.
- [Service Landscape 14](https://bian.org/servicelandscape-14-0-0/).
- [Contrato oficial del SD](https://github.com/bian-official/public/blob/main/release14.0.0/semantic-apis/oas3%20/yamls/PartyReferenceDataDirectory.yaml).
- [Contrato educativo local](customer-profile-bian.yaml).

Se conservan el nombre del archivo y la carpeta para mantener las referencias del repositorio. El contrato educativo pasa a versión 2.0.0 porque sus rutas cambian de CustomerProfile a PartyReferenceDataDirectory y la creación usa Register.

Los DTOs, ContactPreferences, la verificación mediante Execute y sus reglas son adaptaciones educativas. ContactPreferences no es un Behavior Qualifier oficial de este SD; la operación de verificación no representa un proceso KYC oficial BIAN. El HTTP 201 de registro es una adaptación respecto al HTTP 200 de la referencia. Esta API no declara conformidad completa ni certificación BIAN.
