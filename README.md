# Ghostblogger
<?xml version="1.0"?>
<doc>
    <assembly>
        <name>Azure.Data.AppConfiguration</name>
    </assembly>
    <members>
        <member name="T:Azure.Data.AppConfiguration.ConfigurationClient">
            <summary>
            The client to use for interacting with the Azure Configuration Store.
            </summary>
        </member>
        <member name="M:Azure.Data.AppConfiguration.ConfigurationClient.#ctor">
            <summary>
            Protected constructor to allow mocking.
            </summary>
        </member>
        <member name="M:Azure.Data.AppConfiguration.ConfigurationClient.#ctor(System.String)">
            <summary>
            Initializes a new instance of the <see cref="T:Azure.Data.AppConfiguration.ConfigurationClient"/> class.
            </summary>
            <param name="connectionString">Connection string with authentication option and related parameters.</param>
        </member>
        <member name="M:Azure.Data.AppConfiguration.ConfigurationClient.#ctor(System.String,Azure.Data.AppConfiguration.ConfigurationClientOptions)">
            <summary>
            Initializes a new instance of the <see cref="T:Azure.Data.AppConfiguration.ConfigurationClient"/> class.
            </summary>
            <param name="connectionString">Connection string with authentication option and related parameters.</param>
            <param name="options">Options that allow configuration of requests sent to the configuration store.</param>
        </member>
        <member name="M:Azure.Data.AppConfiguration.ConfigurationClient.#ctor(System.Uri,Azure.Core.TokenCredential)">
            <summary>
            Initializes a new instance of the <see cref="T:Azure.Data.AppConfiguration.ConfigurationClient"/> class.
            </summary>
            <param name="endpoint">The <see cref="T:System.Uri"/> referencing the app configuration storage.</param>
            <param name="credential">The token credential used to sign requests.</param>
        </member>
        <member name="M:Azure.Data.AppConfiguration.ConfigurationClient.#ctor(System.Uri,Azure.Core.TokenCredential,Azure.Data.AppConfiguration.ConfigurationClientOptions)">
            <summary>
            Initializes a new instance of the <see cref="T:Azure.Data.AppConfiguration.ConfigurationClient"/> class.
            </summary>
            <param name="endpoint">The <see cref="T:System.Uri"/> referencing the app configuration storage.</param>
            <param name="credential">The token credential used to sign requests.</param>
            <param name="options">Options that allow configuration of requests sent to the configuration store.</param>
        </member>
        <member name="M:Azure.Data.AppConfiguration.ConfigurationClient.AddConfigurationSettingAsync(System.String,System.String,System.String,System.Threading.CancellationToken)">
            <summary>
            Creates a <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> if the setting, uniquely identified by key and label, does not already exist in the configuration store.
            </summary>
            <param name="key">The primary identifier of the configuration setting.</param>
            <param name="value">The configuration setting's value.</param>
            <param name="label">A label used to group this configuration setting with others.</param>
            <param name="cancellationToken">A <see cref="T:System.Threading.CancellationToken"/> controlling the request lifetime.</param>
            <returns>A response containing the added <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/>.</returns>
        </member>
        <member name="M:Azure.Data.AppConfiguration.ConfigurationClient.AddConfigurationSetting(System.String,System.String,System.String,System.Threading.CancellationToken)">
            <summary>
            Creates a <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> if the setting, uniquely identified by key and label, does not already exist in the configuration store.
            </summary>
            <param name="key">The primary identifier of the configuration setting.</param>
            <param name="value">The configuration setting's value.</param>
            <param name="label">A label used to group this configuration setting with others.</param>
            <param name="cancellationToken">A <see cref="T:System.Threading.CancellationToken"/> controlling the request lifetime.</param>
            <returns>A response containing the added <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/>.</returns>
        </member>
        <member name="M:Azure.Data.AppConfiguration.ConfigurationClient.AddConfigurationSettingAsync(Azure.Data.AppConfiguration.ConfigurationSetting,System.Threading.CancellationToken)">
            <summary>
            Creates a <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> only if the setting does not already exist in the configuration store.
            </summary>
            <param name="setting">The <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> to create.</param>
            <param name="cancellationToken">A <see cref="T:System.Threading.CancellationToken"/> controlling the request lifetime.</param>
            <returns>A response containing the added <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/>.</returns>
        </member>
        <member name="M:Azure.Data.AppConfiguration.ConfigurationClient.AddConfigurationSetting(Azure.Data.AppConfiguration.ConfigurationSetting,System.Threading.CancellationToken)">
            <summary>
            Creates a <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> only if the setting does not already exist in the configuration store.
            </summary>
            <param name="setting">The <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> to create.</param>
            <param name="cancellationToken">A <see cref="T:System.Threading.CancellationToken"/> controlling the request lifetime.</param>
            <returns>A response containing the added <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/>.</returns>
        </member>
        <member name="M:Azure.Data.AppConfiguration.ConfigurationClient.SetConfigurationSettingAsync(System.String,System.String,System.String,System.Threading.CancellationToken)">
            <summary>
            Creates a <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/>, uniquely identified by key and label, if it doesn't exist or overwrites the existing setting in the configuration store.
            </summary>
            <param name="key">The primary identifier of the configuration setting.</param>
            <param name="value">The configuration setting's value.</param>
            <param name="label">A label used to group this configuration setting with others.</param>
            <param name="cancellationToken">A <see cref="T:System.Threading.CancellationToken"/> controlling the request lifetime.</param>
            <returns>A response containing the <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> written to the configuration store.</returns>
        </member>
        <member name="M:Azure.Data.AppConfiguration.ConfigurationClient.SetConfigurationSetting(System.String,System.String,System.String,System.Threading.CancellationToken)">
            <summary>
            Creates a <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/>, uniquely identified by key and label, if it doesn't exist or overwrites the existing setting in the configuration store.
            </summary>
            <param name="key">The primary identifier of the configuration setting.</param>
            <param name="value">The configuration setting's value.</param>
            <param name="label">A label used to group this configuration setting with others.</param>
            <param name="cancellationToken">A <see cref="T:System.Threading.CancellationToken"/> controlling the request lifetime.</param>
            <returns>A response containing the <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> written to the configuration store.</returns>
        </member>
        <member name="M:Azure.Data.AppConfiguration.ConfigurationClient.SetConfigurationSettingAsync(Azure.Data.AppConfiguration.ConfigurationSetting,System.Boolean,System.Threading.CancellationToken)">
            <summary>
            Creates a <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> if it doesn't exist or overwrites the existing setting in the configuration store.
            </summary>
            <param name="setting">The <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> to create.</param>
            <param name="onlyIfUnchanged">If set to true and the configuration setting exists in the configuration store, overwrite the setting
            if the passed-in <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> is the same version as the one in the configuration store.  The setting versions
            are the same if their ETag fields match.  If the two settings are different versions, this method will throw an exception to indicate
            that the setting in the configuration store was modified since it was last obtained by the client.</param>
            <param name="cancellationToken">A <see cref="T:System.Threading.CancellationToken"/> controlling the request lifetime.</param>
            <returns>A response containing the <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> written to the configuration store.</returns>
        </member>
        <member name="M:Azure.Data.AppConfiguration.ConfigurationClient.SetConfigurationSetting(Azure.Data.AppConfiguration.ConfigurationSetting,System.Boolean,System.Threading.CancellationToken)">
            <summary>
            Creates a <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> if it doesn't exist or overwrites the existing setting in the configuration store.
            </summary>
            <param name="setting">The <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> to create.</param>
            <param name="onlyIfUnchanged">If set to true and the configuration setting exists in the configuration store, overwrite the setting
            if the passed-in <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> is the same version as the one in the configuration store.  The setting versions
            are the same if their ETag fields match.  If the two settings are different versions, this method will throw an exception to indicate
            that the setting in the configuration store was modified since it was last obtained by the client.</param>
            <param name="cancellationToken">A <see cref="T:System.Threading.CancellationToken"/> controlling the request lifetime.</param>
            <returns>A response containing the <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> written to the configuration store.</returns>
        </member>
        <member name="M:Azure.Data.AppConfiguration.ConfigurationClient.DeleteConfigurationSettingAsync(System.String,System.String,System.Threading.CancellationToken)">
            <summary>
            Delete a <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> from the configuration store.
            </summary>
            <param name="key">The primary identifier of the configuration setting.</param>
            <param name="label">A label used to group this configuration setting with others.</param>
            <param name="cancellationToken">A <see cref="T:System.Threading.CancellationToken"/> controlling the request lifetime.</param>
            <returns>A response indicating the success of the operation.</returns>
        </member>
        <member name="M:Azure.Data.AppConfiguration.ConfigurationClient.DeleteConfigurationSetting(System.String,System.String,System.Threading.CancellationToken)">
            <summary>
            Delete a <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> from the configuration store.
            </summary>
            <param name="key">The primary identifier of the configuration setting.</param>
            <param name="label">A label used to group this configuration setting with others.</param>
            <param name="cancellationToken">A <see cref="T:System.Threading.CancellationToken"/> controlling the request lifetime.</param>
            <returns>A response indicating the success of the operation.</returns>
        </member>
        <member name="M:Azure.Data.AppConfiguration.ConfigurationClient.DeleteConfigurationSettingAsync(Azure.Data.AppConfiguration.ConfigurationSetting,System.Boolean,System.Threading.CancellationToken)">
            <summary>
            Delete a <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> from the configuration store.
            </summary>
            <param name="setting">The <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> to delete.</param>
            <param name="onlyIfUnchanged">If set to true and the configuration setting exists in the configuration store, delete the setting
            if the passed-in <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> is the same version as the one in the configuration store. The setting versions
            are the same if their ETag fields match.  If the two settings are different versions, this method will throw an exception to indicate
            that the setting in the configuration store was modified since it was last obtained by the client.</param>
            <param name="cancellationToken">A <see cref="T:System.Threading.CancellationToken"/> controlling the request lifetime.</param>
            <returns>A response indicating the success of the operation.</returns>
        </member>
        <member name="M:Azure.Data.AppConfiguration.ConfigurationClient.DeleteConfigurationSetting(Azure.Data.AppConfiguration.ConfigurationSetting,System.Boolean,System.Threading.CancellationToken)">
            <summary>
            Delete a <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> from the configuration store.
            </summary>
            <param name="setting">The <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> to delete.</param>
            <param name="onlyIfUnchanged">If set to true and the configuration setting exists in the configuration store, delete the setting
            if the passed-in <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> is the same version as the one in the configuration store. The setting versions
            are the same if their ETag fields match.  If the two settings are different versions, this method will throw an exception to indicate
            that the setting in the configuration store was modified since it was last obtained by the client.</param>
            <param name="cancellationToken">A <see cref="T:System.Threading.CancellationToken"/> controlling the request lifetime.</param>
            <returns>A response indicating the success of the operation.</returns>
        </member>
        <member name="M:Azure.Data.AppConfiguration.ConfigurationClient.GetConfigurationSettingAsync(System.String,System.String,System.Threading.CancellationToken)">
            <summary>
            Retrieve an existing <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/>, uniquely identified by key and label, from the configuration store.
            </summary>
            <param name="key">The primary identifier of the configuration setting to retrieve.</param>
            <param name="label">A label used to group this configuration setting with others.</param>
            <param name="cancellationToken">A <see cref="T:System.Threading.CancellationToken"/> controlling the request lifetime.</param>
            <returns>A response containing the retrieved <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/>.</returns>
        </member>
        <member name="M:Azure.Data.AppConfiguration.ConfigurationClient.GetConfigurationSetting(System.String,System.String,System.Threading.CancellationToken)">
            <summary>
            Retrieve an existing <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/>, uniquely identified by key and label, from the configuration store.
            </summary>
            <param name="key">The primary identifier of the configuration setting to retrieve.</param>
            <param name="label">A label used to group this configuration setting with others.</param>
            <param name="cancellationToken">A <see cref="T:System.Threading.CancellationToken"/> controlling the request lifetime.</param>
            <returns>A response containing the retrieved <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/>.</returns>
        </member>
        <member name="M:Azure.Data.AppConfiguration.ConfigurationClient.GetConfigurationSettingAsync(Azure.Data.AppConfiguration.ConfigurationSetting,System.Boolean,System.Threading.CancellationToken)">
            <summary>
            Retrieve an existing <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> from the configuration store.
            </summary>
            <param name="setting">The <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> to retrieve.</param>
            <param name="onlyIfChanged">If set to true, only retrieve the setting from the configuration store if it has changed since the client last retrieved it.
            It is determined to have changed if the ETag field on the passed-in <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> is different from the ETag of the setting in the
            configuration store.  If it has not changed, the returned response will have have no value, and will throw if response.Value is accessed.  Callers may
            check the status code on the response to avoid triggering the exception.</param>
            <param name="cancellationToken">A <see cref="T:System.Threading.CancellationToken"/> controlling the request lifetime.</param>
            <returns>A response containing the retrieved <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/>.</returns>
        </member>
        <member name="M:Azure.Data.AppConfiguration.ConfigurationClient.GetConfigurationSetting(Azure.Data.AppConfiguration.ConfigurationSetting,System.Boolean,System.Threading.CancellationToken)">
            <summary>
            Retrieve an existing <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> from the configuration store.
            </summary>
            <param name="setting">The <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> to retrieve.</param>
            <param name="onlyIfChanged">If set to true, only retrieve the setting from the configuration store if it has changed since the client last retrieved it.
            It is determined to have changed if the ETag field on the passed-in <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> is different from the ETag of the setting in the
            configuration store.  If it has not changed, the returned response will have have no value, and will throw if response.Value is accessed.  Callers may
            check the status code on the response to avoid triggering the exception.</param>
            <param name="cancellationToken">A <see cref="T:System.Threading.CancellationToken"/> controlling the request lifetime.</param>
            <returns>A response containing the retrieved <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/>.</returns>
        </member>
        <member name="M:Azure.Data.AppConfiguration.ConfigurationClient.GetConfigurationSettingAsync(Azure.Data.AppConfiguration.ConfigurationSetting,System.DateTimeOffset,System.Threading.CancellationToken)">
            <summary>
            Retrieve an existing <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> from the configuration store.
            </summary>
            <param name="setting">The <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> to retrieve.</param>
            <param name="acceptDateTime">The setting will be retrieved exactly as it existed at the provided time.</param>
            <param name="cancellationToken">A <see cref="T:System.Threading.CancellationToken"/> controlling the request lifetime.</param>
            <returns>A response containing the retrieved <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/>.</returns>
        </member>
        <member name="M:Azure.Data.AppConfiguration.ConfigurationClient.GetConfigurationSetting(Azure.Data.AppConfiguration.ConfigurationSetting,System.DateTimeOffset,System.Threading.CancellationToken)">
            <summary>
            Retrieve an existing <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> from the configuration store.
            </summary>
            <param name="setting">The <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> to retrieve.</param>
            <param name="acceptDateTime">The setting will be retrieved exactly as it existed at the provided time.</param>
            <param name="cancellationToken">A <see cref="T:System.Threading.CancellationToken"/> controlling the request lifetime.</param>
            <returns>A response containing the retrieved <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/>.</returns>
        </member>
        <member name="M:Azure.Data.AppConfiguration.ConfigurationClient.GetConfigurationSettingsAsync(Azure.Data.AppConfiguration.SettingSelector,System.Threading.CancellationToken)">
            <summary>
            Retrieves one or more <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> entities that match the options specified in the passed-in <see cref="T:Azure.Data.AppConfiguration.SettingSelector"/>.
            </summary>
            <param name="selector">Options used to select a set of <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> entities from the configuration store.</param>
            <param name="cancellationToken">A <see cref="T:System.Threading.CancellationToken"/> controlling the request lifetime.</param>
            <returns>An enumerable collection containing the retrieved <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> entities.</returns>
        </member>
        <member name="M:Azure.Data.AppConfiguration.ConfigurationClient.GetConfigurationSettings(Azure.Data.AppConfiguration.SettingSelector,System.Threading.CancellationToken)">
            <summary>
            Retrieves one or more <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> entities that match the options specified in the passed-in <see cref="T:Azure.Data.AppConfiguration.SettingSelector"/>.
            </summary>
            <param name="selector">Set of options for selecting <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> from the configuration store.</param>
            <param name="cancellationToken">A <see cref="T:System.Threading.CancellationToken"/> controlling the request lifetime.</param>
        </member>
        <member name="M:Azure.Data.AppConfiguration.ConfigurationClient.GetRevisionsAsync(System.String,System.String,System.Threading.CancellationToken)">
            <summary>
            Retrieves the revisions of one or more <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> entities that match the specified <paramref name="keyFilter"/> and <paramref name="labelFilter"/>.
            </summary>
            <param name="keyFilter">Key filter that will be used to select a set of <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> entities.</param>
            <param name="labelFilter">Label filter that will be used to select a set of <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> entities.</param>
            <param name="cancellationToken">A <see cref="T:System.Threading.CancellationToken"/> controlling the request lifetime.</param>
        </member>
        <member name="M:Azure.Data.AppConfiguration.ConfigurationClient.GetRevisions(System.String,System.String,System.Threading.CancellationToken)">
            <summary>
            Retrieves the revisions of one or more <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> entities that match the specified <paramref name="keyFilter"/> and <paramref name="labelFilter"/>.
            </summary>
            <param name="keyFilter">Key filter that will be used to select a set of <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> entities.</param>
            <param name="labelFilter">Label filter that will be used to select a set of <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> entities.</param>
            <param name="cancellationToken">A <see cref="T:System.Threading.CancellationToken"/> controlling the request lifetime.</param>
        </member>
        <member name="M:Azure.Data.AppConfiguration.ConfigurationClient.GetRevisionsAsync(Azure.Data.AppConfiguration.SettingSelector,System.Threading.CancellationToken)">
            <summary>
            Retrieves the revisions of one or more <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> entities that satisfy the options of the <see cref="T:Azure.Data.AppConfiguration.SettingSelector"/>.
            </summary>
            <param name="selector">Set of options for selecting <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> from the configuration store.</param>
            <param name="cancellationToken">A <see cref="T:System.Threading.CancellationToken"/> controlling the request lifetime.</param>
        </member>
        <member name="M:Azure.Data.AppConfiguration.ConfigurationClient.GetRevisions(Azure.Data.AppConfiguration.SettingSelector,System.Threading.CancellationToken)">
            <summary>
            Retrieves the revisions of one or more <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> entities that satisfy the options of the <see cref="T:Azure.Data.AppConfiguration.SettingSelector"/>.
            </summary>
            <param name="selector">Set of options for selecting <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> from the configuration store.</param>
            <param name="cancellationToken">A <see cref="T:System.Threading.CancellationToken"/> controlling the request lifetime.</param>
        </member>
        <member name="M:Azure.Data.AppConfiguration.ConfigurationClient.GetConfigurationSettingsPageAsync(Azure.Data.AppConfiguration.SettingSelector,System.String,System.Threading.CancellationToken)">
            <summary>
            Fetches the <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> from the configuration store that match the options selected in the <see cref="T:Azure.Data.AppConfiguration.SettingSelector"/>.
            </summary>
            <param name="selector">Set of options for selecting settings from the configuration store.</param>
            <param name="pageLink"></param>
            <param name="cancellationToken">A <see cref="T:System.Threading.CancellationToken"/> controlling the request lifetime.</param>
        </member>
        <member name="M:Azure.Data.AppConfiguration.ConfigurationClient.GetConfigurationSettingsPage(Azure.Data.AppConfiguration.SettingSelector,System.String,System.Threading.CancellationToken)">
            <summary>
            Fetches the <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> from the configuration store that match the options selected in the <see cref="T:Azure.Data.AppConfiguration.SettingSelector"/>.
            </summary>
            <param name="selector">Set of options for selecting settings from the configuration store.</param>
            <param name="pageLink"></param>
            <param name="cancellationToken">A <see cref="T:System.Threading.CancellationToken"/> controlling the request lifetime.</param>
        </member>
        <member name="M:Azure.Data.AppConfiguration.ConfigurationClient.GetRevisionsPageAsync(Azure.Data.AppConfiguration.SettingSelector,System.String,System.Threading.CancellationToken)">
            <summary>
            Lists chronological/historical representation of <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> from the configuration store that match the options selected in the <see cref="T:Azure.Data.AppConfiguration.SettingSelector"/>.
            </summary>
            <remarks>Revisions are provided in descending order from their respective <see cref="P:Azure.Data.AppConfiguration.ConfigurationSetting.LastModified"/> date.</remarks>
            <param name="selector">Set of options for selecting settings from the configuration store.</param>
            <param name="pageLink"></param>
            <param name="cancellationToken">A <see cref="T:System.Threading.CancellationToken"/> controlling the request lifetime.</param>
        </member>
        <member name="M:Azure.Data.AppConfiguration.ConfigurationClient.GetRevisionsPage(Azure.Data.AppConfiguration.SettingSelector,System.String,System.Threading.CancellationToken)">
            <summary>
            Lists chronological/historical representation of <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> from the configuration store that match the options selected in the <see cref="T:Azure.Data.AppConfiguration.SettingSelector"/>.
            </summary>
            <remarks>Revisions are provided in descending order from their respective <see cref="P:Azure.Data.AppConfiguration.ConfigurationSetting.LastModified"/> date.</remarks>
            <param name="selector">Set of options for selecting settings from the configuration store.</param>
            <param name="pageLink"></param>
            <param name="cancellationToken">A <see cref="T:System.Threading.CancellationToken"/> controlling the request lifetime.</param>
        </member>
        <member name="M:Azure.Data.AppConfiguration.ConfigurationClient.SetReadOnlyAsync(System.String,System.Boolean,System.Threading.CancellationToken)">
            <summary>
            Sets an existing <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> to read only or read write state in the configuration store.
            </summary>
            <param name="key">The primary identifier of the configuration setting.</param>
            <param name="isReadOnly">If true, the <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> will be set to read only in the configuration store. If false, it will be set to read write.</param>
            <param name="cancellationToken">A <see cref="T:System.Threading.CancellationToken"/> controlling the request lifetime.</param>
        </member>
        <member name="M:Azure.Data.AppConfiguration.ConfigurationClient.SetReadOnly(System.String,System.Boolean,System.Threading.CancellationToken)">
            <summary>
            Sets an existing <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> to read only or read write state in the configuration store.
            </summary>
            <param name="key">The primary identifier of the configuration setting.</param>
            <param name="isReadOnly">If true, the <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> will be set to read only in the configuration store. If false, it will be set to read write.</param>
            <param name="cancellationToken">A <see cref="T:System.Threading.CancellationToken"/> controlling the request lifetime.</param>
        </member>
        <member name="M:Azure.Data.AppConfiguration.ConfigurationClient.SetReadOnlyAsync(System.String,System.String,System.Boolean,System.Threading.CancellationToken)">
            <summary>
            Sets an existing <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> to read only or read write state in the configuration store.
            </summary>
            <param name="key">The primary identifier of the configuration setting.</param>
            <param name="label">A label used to group this configuration setting with others.</param>
            <param name="isReadOnly">If true, the <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> will be set to read only in the configuration store. If false, it will be set to read write.</param>
            <param name="cancellationToken">A <see cref="T:System.Threading.CancellationToken"/> controlling the request lifetime.</param>
        </member>
        <member name="M:Azure.Data.AppConfiguration.ConfigurationClient.SetReadOnly(System.String,System.String,System.Boolean,System.Threading.CancellationToken)">
            <summary>
            Sets an existing <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> to read only or read write state in the configuration store.
            </summary>
            <param name="key">The primary identifier of the configuration setting.</param>
            <param name="label">A label used to group this configuration setting with others.</param>
            <param name="isReadOnly">If true, the <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> will be set to read only in the configuration store. If false, it will be set to read write.</param>
            <param name="cancellationToken">A <see cref="T:System.Threading.CancellationToken"/> controlling the request lifetime.</param>
        </member>
        <member name="M:Azure.Data.AppConfiguration.ConfigurationClient.Equals(System.Object)">
            <summary>
            Check if two ConfigurationSetting instances are equal.
            </summary>
            <param name="obj">The instance to compare to.</param>
        </member>
        <member name="M:Azure.Data.AppConfiguration.ConfigurationClient.GetHashCode">
            <summary>
            Get a hash code for the ConfigurationSetting.
            </summary>
        </member>
        <member name="M:Azure.Data.AppConfiguration.ConfigurationClient.ToString">
            <summary>
            Creates a Key Value string in reference to the ConfigurationSetting.
            </summary>
        </member>
        <member name="T:Azure.Data.AppConfiguration.ConfigurationClientOptions">
            <summary>
            Options that allow users to configure the requests sent to the App Configuration service.
            </summary>
        </member>
        <member name="F:Azure.Data.AppConfiguration.ConfigurationClientOptions.LatestVersion">
            <summary>
            The latest service version supported by this client library.
            </summary>
        </member>
        <member name="T:Azure.Data.AppConfiguration.ConfigurationClientOptions.ServiceVersion">
            <summary>
            The versions of the App Configuration service supported by this client library.
            </summary>
        </member>
        <member name="F:Azure.Data.AppConfiguration.ConfigurationClientOptions.ServiceVersion.V1_0">
            <summary>
            Version 1.0.
            </summary>
        </member>
        <member name="P:Azure.Data.AppConfiguration.ConfigurationClientOptions.Version">
            <summary>
            Gets the <see cref="T:Azure.Data.AppConfiguration.ConfigurationClientOptions.ServiceVersion"/> of the service API used when
            making requests.
            </summary>
        </member>
        <member name="M:Azure.Data.AppConfiguration.ConfigurationClientOptions.#ctor(Azure.Data.AppConfiguration.ConfigurationClientOptions.ServiceVersion)">
            <summary>
            Initializes a new instance of the <see cref="T:Azure.Data.AppConfiguration.ConfigurationClientOptions"/>
            class.
            </summary>
            <param name="version">
            The <see cref="T:Azure.Data.AppConfiguration.ConfigurationClientOptions.ServiceVersion"/> of the service API used when
            making requests.
            </param>
        </member>
        <member name="T:Azure.Data.AppConfiguration.ConfigurationModelFactory">
            <summary>
            Configuration Setting model factory that enables mocking for the App Configuration client library.
            </summary>
        </member>
        <member name="M:Azure.Data.AppConfiguration.ConfigurationModelFactory.ConfigurationSetting(System.String,System.String,System.String,System.String,Azure.ETag,System.Nullable{System.DateTimeOffset},System.Nullable{System.Boolean})">
            <summary>
            Initializes a new instance of the <see cref="M:Azure.Data.AppConfiguration.ConfigurationModelFactory.ConfigurationSetting(System.String,System.String,System.String,System.String,Azure.ETag,System.Nullable{System.DateTimeOffset},System.Nullable{System.Boolean})"/> for mocking purposes.
            </summary>
            <param name="key">The primary identifier of a configuration setting.</param>
            <param name="value">The configuration setting's value.</param>
            <param name="label">A label used to group configuration settings.</param>
            <param name="contentType">The content type of the configuration setting's value.</param>
            <param name="eTag">An ETag indicating the version of a configuration setting within a configuration store.</param>
            <param name="lastModified">The last time a modifying operation was performed on the given configuration setting.</param>
            <param name="isReadOnly">A value indicating whether the configuration setting is read only.</param>
        </member>
        <member name="T:Azure.Data.AppConfiguration.ConfigurationSetting">
            <summary>
            A setting, defined by a unique combination of a key and label.
            </summary>
        </member>
        <member name="M:Azure.Data.AppConfiguration.ConfigurationSetting.#ctor(System.String,System.String,System.String)">
            <summary>
            Creates a configuration setting and sets the values from the passed in parameter to this setting.
            </summary>
            <param name="key">The primary identifier of the configuration setting.</param>
            <param name="value">The configuration setting's value.</param>
            <param name="label">A label used to group this configuration setting with others.</param>
        </member>
        <member name="P:Azure.Data.AppConfiguration.ConfigurationSetting.Key">
            <summary>
            The primary identifier of the configuration setting.
            A <see cref="P:Azure.Data.AppConfiguration.ConfigurationSetting.Key"/> is used together with a <see cref="P:Azure.Data.AppConfiguration.ConfigurationSetting.Label"/> to uniquely identify a configuration setting.
            </summary>
        </member>
        <member name="P:Azure.Data.AppConfiguration.ConfigurationSetting.Label">
            <summary>
            A value used to group configuration settings.
            A <see cref="P:Azure.Data.AppConfiguration.ConfigurationSetting.Label"/> is used together with a <see cref="P:Azure.Data.AppConfiguration.ConfigurationSetting.Key"/> to uniquely identify a configuration setting.
            </summary>
        </member>
        <member name="P:Azure.Data.AppConfiguration.ConfigurationSetting.Value">
            <summary>
            The configuration setting's value.
            </summary>
        </member>
        <member name="P:Azure.Data.AppConfiguration.ConfigurationSetting.ContentType">
            <summary>
            The content type of the configuration setting's value.
            Providing a proper content-type can enable transformations of values when they are retrieved by applications.
            </summary>
        </member>
        <member name="P:Azure.Data.AppConfiguration.ConfigurationSetting.ETag">
            <summary>
            An ETag indicating the state of a configuration setting within a configuration store.
            </summary>
        </member>
        <member name="P:Azure.Data.AppConfiguration.ConfigurationSetting.LastModified">
            <summary>
            The last time a modifying operation was performed on the given configuration setting.
            </summary>
        </member>
        <member name="P:Azure.Data.AppConfiguration.ConfigurationSetting.IsReadOnly">
            <summary>
            A value indicating whether the configuration setting is read only.
            A read only configuration setting may not be modified until it is made writable.
            </summary>
        </member>
        <member name="P:Azure.Data.AppConfiguration.ConfigurationSetting.Tags">
            <summary>
            A dictionary of tags used to assign additional properties to a configuration setting.
            These can be used to indicate how a configuration setting may be applied.
            </summary>
        </member>
        <member name="M:Azure.Data.AppConfiguration.ConfigurationSetting.Equals(System.Object)">
            <summary>
            Check if two ConfigurationSetting instances are equal.
            </summary>
            <param name="obj">The instance to compare to.</param>
        </member>
        <member name="M:Azure.Data.AppConfiguration.ConfigurationSetting.GetHashCode">
            <summary>
            Get a hash code for the ConfigurationSetting.
            </summary>
        </member>
        <member name="M:Azure.Data.AppConfiguration.ConfigurationSetting.ToString">
            <summary>
            Creates a (Key,Value) string in reference to the ConfigurationSetting.
            </summary>
        </member>
        <member name="T:Azure.Data.AppConfiguration.SettingFields">
            <summary>
            Fields to retrieve from a configuration setting.
            </summary>
        </member>
        <member name="F:Azure.Data.AppConfiguration.SettingFields.Key">
            <summary>
            The primary identifier of a configuration setting.
            </summary>
        </member>
        <member name="F:Azure.Data.AppConfiguration.SettingFields.Label">
            <summary>
            A label used to group configuration settings.
            </summary>
        </member>
        <member name="F:Azure.Data.AppConfiguration.SettingFields.Value">
            <summary>
            The value of the configuration setting.
            </summary>
        </member>
        <member name="F:Azure.Data.AppConfiguration.SettingFields.ContentType">
            <summary>
            The content type of the configuration setting's value.
            </summary>
        </member>
        <member name="F:Azure.Data.AppConfiguration.SettingFields.ETag">
            <summary>
            An ETag indicating the version of a configuration setting within a configuration store.
            </summary>
        </member>
        <member name="F:Azure.Data.AppConfiguration.SettingFields.LastModified">
            <summary>
            >The last time a modifying operation was performed on the given configuration setting.
            </summary>
        </member>
        <member name="F:Azure.Data.AppConfiguration.SettingFields.IsReadOnly">
            <summary>
            A value indicating whether the configuration setting is read-only.
            </summary>
        </member>
        <member name="F:Azure.Data.AppConfiguration.SettingFields.Tags">
            <summary>
            A dictionary of tags that can help identify what a configuration setting may be applicable for.
            </summary>
        </member>
        <member name="F:Azure.Data.AppConfiguration.SettingFields.All">
            <summary>
            Allows for all the properties of a ConfigurationSetting to be retrieved.
            </summary>
        </member>
        <member name="T:Azure.Data.AppConfiguration.SettingSelector">
            <summary>
            <para><see cref="T:Azure.Data.AppConfiguration.SettingSelector"/> is a set of options that allows selecting
            a filtered set of <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> entities from the
            configuration store, and optionally allows indicating which fields of
            each setting to retrieve.</para>
            <para>Literals or filters may be specified for keys and labels.</para>
            <para>For more information, <see href="https://github.com/Azure/AppConfiguration/blob/master/docs/REST/kv.md#filtering">Filtering</see>.</para>
            </summary>
        </member>
        <member name="F:Azure.Data.AppConfiguration.SettingSelector.Any">
            <summary>
            A wildcard that matches any key or any label when passed as a filter
            to Keys or Labels.
            </summary>
        </member>
        <member name="P:Azure.Data.AppConfiguration.SettingSelector.KeyFilter">
            <summary>
            Key filter that will be used to select a set of <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> entities.
            </summary>
            <remarks>See the documentation for this client library for details on the format of filter expressions.</remarks>
        </member>
        <member name="P:Azure.Data.AppConfiguration.SettingSelector.LabelFilter">
            <summary>
            Label filter that will be used to select a set of <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> entities.
            </summary>
            <remarks>See the documentation for this client library for details on the format of filter expressions.</remarks>
        </member>
        <member name="P:Azure.Data.AppConfiguration.SettingSelector.Fields">
            <summary>
            The fields of the <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> to retrieve for each setting in the retrieved group.
            </summary>
        </member>
        <member name="P:Azure.Data.AppConfiguration.SettingSelector.AcceptDateTime">
            <summary>
            Indicates the point in time in the revision history of the selected <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> entities to retrieve.
            If set, all properties of the <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> entities in the returned group will be exactly what they
            were at this time.
            </summary>
        </member>
        <member name="M:Azure.Data.AppConfiguration.SettingSelector.#ctor">
            <summary>
            Creates a default <see cref="T:Azure.Data.AppConfiguration.SettingSelector"/> that will retrieve all <see cref="T:Azure.Data.AppConfiguration.ConfigurationSetting"/> entities in the configuration store.
            </summary>
        </member>
        <member name="M:Azure.Data.AppConfiguration.SettingSelector.Equals(System.Object)">
            <summary>
            Check if two SettingSelector instances are equal.
            </summary>
            <param name="obj">The instance to compare to.</param>
        </member>
        <member name="M:Azure.Data.AppConfiguration.SettingSelector.GetHashCode">
            <summary>
            Get a hash code for the SettingSelector.
            </summary>
        </member>
        <member name="M:Azure.Data.AppConfiguration.SettingSelector.ToString">
            <summary>
            Creates a string in reference to the SettingSelector.
            </summary>
        </member>
        <member name="P:Azure.Data.AppConfiguration.SyncToken.Id">
            <summary>
            The token's ID.
            </summary>
        </member>
        <member name="P:Azure.Data.AppConfiguration.SyncToken.Value">
            <summary>
            The token's value.
            </summary>
        </member>
        <member name="P:Azure.Data.AppConfiguration.SyncToken.SequenceNumber">
            <summary>
            Token sequence number (version). Higher means newer version of the same token.
            </summary>
        </member>
        <member name="M:Azure.Data.AppConfiguration.SyncToken.ToString">
            <summary>
            Creates a string representation of a <see cref="T:Azure.Data.AppConfiguration.SyncToken"/>.
            </summary>
        </member>
        <member name="T:Azure.Core.Argument">
            <summary>
            Argument validation.
            </summary>
            <remarks>
              <para>This class should be shared via source using Azure.Core.props and contain only common argument validation.
                It is declared partial so that you can use the same familiar class name but extend it with project-specific validation.
                To extend the functionality of this class, just declare your own partial <see cref="T:Azure.Core.Argument"/> class with project-specific methods.
              </para>
              <para>
                Be sure to document exceptions thrown by these methods on your public methods.
              </para>
            </remarks>
        </member>
        <member name="M:Azure.Core.Argument.AssertNotNull``1(``0,System.String)">
            <summary>
            Throws if <paramref name="value"/> is null.
            </summary>
            <param name="value">The value to validate.</param>
            <param name="name">The name of the parameter.</param>
            <exception cref="T:System.ArgumentNullException"><paramref name="value"/> is null.</exception>
        </member>
        <member name="M:Azure.Core.Argument.AssertNotNull``1(System.Nullable{``0},System.String)">
            <summary>
            Throws if <paramref name="value"/> has not been initialized.
            </summary>
            <param name="value">The value to validate.</param>
            <param name="name">The name of the parameter.</param>
            <exception cref="T:System.ArgumentNullException"><paramref name="value"/> has not been initialized.</exception>
        </member>
        <member name="M:Azure.Core.Argument.AssertNotNullOrEmpty``1(System.Collections.Generic.IEnumerable{``0},System.String)">
            <summary>
            Throws if <paramref name="value"/> is null or an empty collection.
            </summary>
            <param name="value">The value to validate.</param>
            <param name="name">The name of the parameter.</param>
            <exception cref="T:System.ArgumentException"><paramref name="value"/> is an empty collection.</exception>
            <exception cref="T:System.ArgumentNullException"><paramref name="value"/> is null.</exception>
        </member>
        <member name="M:Azure.Core.Argument.AssertNotNullOrEmpty(System.String,System.String)">
            <summary>
            Throws if <paramref name="value"/> is null or an empty string.
            </summary>
            <param name="value">The value to validate.</param>
            <param name="name">The name of the parameter.</param>
            <exception cref="T:System.ArgumentException"><paramref name="value"/> is an empty string.</exception>
            <exception cref="T:System.ArgumentNullException"><paramref name="value"/> is null.</exception>
        </member>
        <member name="M:Azure.Core.Argument.AssertNotNullOrWhiteSpace(System.String,System.String)">
            <summary>
            Throws if <paramref name="value"/> is null, an empty string, or consists only of white-space characters.
            </summary>
            <param name="value">The value to validate.</param>
            <param name="name">The name of the parameter.</param>
            <exception cref="T:System.ArgumentException"><paramref name="value"/> is an empty string or consists only of white-space characters.</exception>
            <exception cref="T:System.ArgumentNullException"><paramref name="value"/> is null.</exception>
        </member>
        <member name="M:Azure.Core.Argument.AssertNotDefault``1(``0@,System.String)">
            <summary>
            Throws if <paramref name="value"/> is the default value for type <typeparamref name="T"/>.
            </summary>
            <typeparam name="T">The type of structure to validate which implements <see cref="T:System.IEquatable`1"/>.</typeparam>
            <param name="value">The value to validate.</param>
            <param name="name">The name of the parameter.</param>
            <exception cref="T:System.ArgumentException"><paramref name="value"/> is the default value for type <typeparamref name="T"/>.</exception>
        </member>
        <member name="M:Azure.Core.Argument.AssertInRange``1(``0,``0,``0,System.String)">
            <summary>
            Throws if <paramref name="value"/> is less than the <paramref name="minimum"/> or greater than the <paramref name="maximum"/>.
            </summary>
            <typeparam name="T">The type of to validate which implements <see cref="T:System.IComparable`1"/>.</typeparam>
            <param name="value">The value to validate.</param>
            <param name="minimum">The minimum value to compare.</param>
            <param name="maximum">The maximum value to compare.</param>
            <param name="name">The name of the parameter.</param>
        </member>
        <member name="T:Azure.Core.AzureResourceProviderNamespaceAttribute">
            <summary>
            This attribute should be set on all client assemblies with value of one of the resource providers
            from the https://docs.microsoft.com/en-us/azure/azure-resource-manager/management/azure-services-resource-providers list.
            </summary>
        </member>
        <member name="T:Azure.Core.ArrayBufferWriter`1">
            <summary>
            Represents a heap-based, array-backed output sink into which <typeparam name="T"/> data can be written.
            </summary>
        </member>
        <member name="M:Azure.Core.ArrayBufferWriter`1.#ctor">
            <summary>
            Creates an instance of an <see cref="T:Azure.Core.ArrayBufferWriter`1"/>, in which data can be written to,
            with the default initial capacity.
            </summary>
        </member>
        <member name="M:Azure.Core.ArrayBufferWriter`1.#ctor(System.Int32)">
            <summary>
            Creates an instance of an <see cref="T:Azure.Core.ArrayBufferWriter`1"/>, in which data can be written to,
            with an initial capacity specified.
            </summary>
            <param name="initialCapacity">The minimum capacity with which to initialize the underlying buffer.</param>
            <exception cref="T:System.ArgumentException">
            Thrown when <paramref name="initialCapacity"/> is not positive (i.e. less than or equal to 0).
            </exception>
        </member>
        <member name="P:Azure.Core.ArrayBufferWriter`1.WrittenMemory">
            <summary>
            Returns the data written to the underlying buffer so far, as a <see cref="T:System.ReadOnlyMemory`1"/>.
            </summary>
        </member>
        <member name="P:Azure.Core.ArrayBufferWriter`1.WrittenSpan">
            <summary>
            Returns the data written to the underlying buffer so far, as a <see cref="T:System.ReadOnlySpan`1"/>.
            </summary>
        </member>
        <member name="P:Azure.Core.ArrayBufferWriter`1.WrittenCount">
            <summary>
            Returns the amount of data written to the underlying buffer so far.
            </summary>
        </member>
        <member name="P:Azure.Core.ArrayBufferWriter`1.Capacity">
            <summary>
            Returns the total amount of space within the underlying buffer.
            </summary>
        </member>
        <member name="P:Azure.Core.ArrayBufferWriter`1.FreeCapacity">
            <summary>
            Returns the amount of space available that can still be written into without forcing the underlying buffer to grow.
            </summary>
        </member>
        <member name="M:Azure.Core.ArrayBufferWriter`1.Clear">
            <summary>
            Clears the data written to the underlying buffer.
            </summary>
            <remarks>
            You must clear the <see cref="T:Azure.Core.ArrayBufferWriter`1"/> before trying to re-use it.
            </remarks>
        </member>
        <member name="M:Azure.Core.ArrayBufferWriter`1.Advance(System.Int32)">
            <summary>
            Notifies <see cref="T:System.Buffers.IBufferWriter`1"/> that <paramref name="count"/> amount of data was written to the output <see cref="T:System.Span`1"/>/<see cref="T:System.Memory`1"/>.
            </summary>
            <exception cref="T:System.ArgumentException">
            Thrown when <paramref name="count"/> is negative.
            </exception>
            <exception cref="T:System.InvalidOperationException">
            Thrown when attempting to advance past the end of the underlying buffer.
            </exception>
            <remarks>
            You must request a new buffer after calling Advance to continue writing more data and cannot write to a previously acquired buffer.
            </remarks>
        </member>
        <member name="M:Azure.Core.ArrayBufferWriter`1.GetMemory(System.Int32)">
            <summary>
            Returns a <see cref="T:System.Memory`1"/> to write to that is at least the requested length (specified by <paramref name="sizeHint"/>).
            If no <paramref name="sizeHint"/> is provided (or it's equal to <code>0</code>), some non-empty buffer is returned.
            </summary>
            <exception cref="T:System.ArgumentException">
            Thrown when <paramref name="sizeHint"/> is negative.
            </exception>
            <remarks>
            This will never return an empty <see cref="T:System.Memory`1"/>.
            </remarks>
            <remarks>
            There is no guarantee that successive calls will return the same buffer or the same-sized buffer.
            </remarks>
            <remarks>
            You must request a new buffer after calling Advance to continue writing more data and cannot write to a previously acquired buffer.
            </remarks>
        </member>
        <member name="M:Azure.Core.ArrayBufferWriter`1.GetSpan(System.Int32)">
            <summary>
            Returns a <see cref="T:System.Span`1"/> to write to that is at least the requested length (specified by <paramref name="sizeHint"/>).
            If no <paramref name="sizeHint"/> is provided (or it's equal to <code>0</code>), some non-empty buffer is returned.
            </summary>
            <exception cref="T:System.ArgumentException">
            Thrown when <paramref name="sizeHint"/> is negative.
            </exception>
            <remarks>
            This will never return an empty <see cref="T:System.Span`1"/>.
            </remarks>
            <remarks>
            There is no guarantee that successive calls will return the same buffer or the same-sized buffer.
            </remarks>
            <remarks>
            You must request a new buffer after calling Advance to continue writing more data and cannot write to a previously acquired buffer.
            </remarks>
        </member>
        <member name="T:Azure.Core.Pipeline.ActivityExtensions">
            <summary>
            HACK HACK HACK. Some runtime environments like Azure.Functions downgrade System.Diagnostic.DiagnosticSource package version causing method not found exceptions in customer apps
            This type is a temporary workaround to avoid the issue.
            </summary>
        </member>
        <member name="T:Azure.Core.Pipeline.TaskExtensions.Enumerable`1">
            <summary>
            Both <see cref="T:Azure.Core.Pipeline.TaskExtensions.Enumerable`1"/> and <see cref="T:Azure.Core.Pipeline.TaskExtensions.Enumerator`1"/> are defined as public structs so that foreach can use duck typing
            to call <see cref="M:Azure.Core.Pipeline.TaskExtensions.Enumerable`1.GetEnumerator"/> and avoid heap memory allocation.
            Please don't delete this method and don't make these types private.
            </summary>
            <typeparam name="T"></typeparam>
        </member>
        <member name="T:Azure.Core.HashCodeBuilder">
            <summary>
            Copied from https://github.com/dotnet/corefx/blob/master/src/Common/src/CoreLib/System/HashCode.cs.
            </summary>
        </member>
        <member name="T:Microsoft.Extensions.Azure.ConfigurationClientBuilderExtensions">
            <summary>
            Extension methods to add <see cref="T:Azure.Data.AppConfiguration.ConfigurationClient"/> client to clients builder.
            </summary>
        </member>
        <member name="M:Microsoft.Extensions.Azure.ConfigurationClientBuilderExtensions.AddConfigurationClient``1(``0,System.String)">
            <summary>
            Registers a <see cref="T:Azure.Data.AppConfiguration.ConfigurationClient"/> instance with the provided <paramref name="connectionString"/>.
            </summary>
        </member>
        <member name="M:Microsoft.Extensions.Azure.ConfigurationClientBuilderExtensions.AddConfigurationClient``2(``0,``1)">
            <summary>
            Registers a <see cref="T:Azure.Data.AppConfiguration.ConfigurationClient"/> instance with connection options loaded from the provided <paramref name="configuration"/> instance.
            </summary>
        </member>
    </members>
</doc>
