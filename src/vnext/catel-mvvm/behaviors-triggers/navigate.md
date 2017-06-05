# Navigate

Note that this behavior is only available for WPF

The Hyperlink control in WPF is very powerful, but it is hard to make them work outside pages.

Add the following XML namespaces:

``` {.java data-syntaxhighlighter-params="brush: java; gutter: false; theme: Confluence" data-theme="Confluence" style="brush: java; gutter: false; theme: Confluence"}
xmlns:i="clr-namespace:System.Windows.Interactivity;assembly=System.Windows.Interactivity"
xmlns:catel="http://catel.codeplex.com"
```

To execute the NavigateUrl, simply use the behavior as shown below:

``` {.java data-syntaxhighlighter-params="brush: java; gutter: false; theme: Confluence" data-theme="Confluence" style="brush: java; gutter: false; theme: Confluence"}
<TextBlock>
    <Hyperlink NavigateUri="http://catel.codeplex.com">
        <i:Interaction.Behaviors>
            <catel:Navigate />
        </i:Interaction.Behaviors>

        <TextBlock Text="The best MVVM Framework" />
    </Hyperlink>
</TextBlock>
```

Another alternative is to use the LinkLabel control
