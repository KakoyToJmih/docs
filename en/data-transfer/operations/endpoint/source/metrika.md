---
noIndex: true
---

# Configuring source endpoints {{ metrika-endpoint }}

When [creating](../index.md#create) or [updating](../index.md#update) an endpoint, configure access to [{{ metrika }}](https://metrika.yandex.ru/).

## Settings {#settings}

{% list tabs %}

- Management console

   * **Tag numbers**: Specify the [numbers of the tags](https://yandex.ru/support/metrica/general/tag-id.html) the data will be coming from.
   * **Token**: Specify the token required to access the tags. To obtain it, follow [this link](https://oauth.yandex.ru/authorize?response_type=token&client_id=36b7fc9aa96c4fa09158bcacbbdc796a).
   * **Hits**: Select whether information about hits should be transferred.
      * **Fields**: Select the hit fields to export. In addition to the fields you select, there are certain mandatory fields that are always exported.
   * **Sessions**: Select whether information about sessions (visits) should be transferred.
      * **Fields**: Select the session fields to export. In addition to the fields you select, there are certain mandatory fields that are always exported.

{% endlist %}

For more information about the settings, see the [service documentation](https://yandex.ru/support/metrica/index.html).

See [this tutorial](../../../tutorials/metrika-to-clickhouse.md) on how to transfer {{ metrika }} tag data to a {{ CH }} cluster.