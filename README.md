workTest (Mule 4)

- Flow: `get-address` (src/main/mule/get-address.xml)
- Tests: `src/test/munit/get-address-test.xml`

Notes
- Numeric validation uses `^\d+$` for consumer agency ID.
- Address payload is always built after the scatter-gather; `isPrimary` is set when a primary address exists and matches.
- DB calls are mocked in MUnit tests.

Run tests
- In Anypoint Studio: Run MUnit Suite
- Maven: `mvn -DskipTests=false test`
  - If Mule/Anypoint repos require credentials, run tests from Studio where runtime is available.

