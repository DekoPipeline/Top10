# +R リスクに関する注記

## 本資料は、弱点として表れるリスクについてです

Top 10のリスク格付手法は、[OWASP Risk Rating Methodology](https://www.owasp.org/index.php/OWASP_Risk_Rating_Methodology)に基づいています。我々は各Top 10のカテゴリに対して、典型的なWebアプリケーションのそれぞれの弱点について、一般的な発生可能性と影響要素をみて、リスクを推計しました。そしてアプリケーションに対してもっとも重大なリスクをもたらすような弱点に基づいてTop 10を整理しました。これらの要素は、物事が変化し進化するにつれて、新しいTop 10がリリースされる度に更新されます。

[OWASP Risk Rating Methodology](https://www.owasp.org/index.php/OWASP_Risk_Rating_Methodology)は脆弱性のリスクを計算するために、多数の要素を定義しています。但し、実際のアプリケーションやAPIにおける特定の脆弱性よりも、Top 10は一般論を議論すべきです。従って、我々は、リスク計算においてアプリケーションオーナーまたは管理者より、精緻になることはありません。アプリケーションとデータの重要性、脅威の内容、システムの構築方法や運用などに合わせ、ご自身で判断する必要があります。

我々が使用している手法は、弱点の発生可能性に関する三つの要素（普及度、攻撃検知のしやすさ、悪用の容易性）と一つの影響要素（技術的影響）を含めています。各要素のリスクの尺度は、各要素に特有の用語を用いて、1-低から3-高までの範囲です。弱点の「普及度」は計算する時に、必ずしも含む必要はありません。「普及度」データについて、いくもの組織（25ページの謝辞参照）から統計資料の提供を受け、それらの「普及度」に関するデータをまとめ上げ、「普及度」によるTop 10の存在可能性リストを作成しました。このデータは、他の二つの発生可能性に関する要素（攻撃検知のしやすさ、悪用の容易性）と合わせて、各弱点の発生可能性の格付を計算しました。発生可能性の評価においては、我々が推計した「技術的影響」の平均値から、Top 10各項目のリスク順位の全体像を生成しました。（高いほど高リスク）。攻撃検知のしやすさ、悪用の容易性、影響度は、Top 10のそれぞれのカテゴリーに関連して報告されたCVEを分析して計算されました。

**注記**:このアプローチが「脅威エージェント」の可能性を考慮していないことに注意して下さい。また、特定のアプリケーションの技術的な詳細も考慮していません。攻撃者が特定の脆弱性に攻撃する際に、これらの要素が全体の発生可能性に大幅な影響を与える可能性があります。この評価はあなたのビジネスへの実際の影響も考慮していません。あなたの組織の文化、業界、規制などを考慮して、どのぐらいのセキュリティリスクをアプリケーションとAPIに対して負うかを決定して下さい。OWASP Top 10の目的は、特定のアプリケーションやAPIを想定したリスク分析ではありません。

以下に、**A6:2017-Security Misconfiguration**を例として、我々の計算を示します。

![Risk Calculation for A6:2017-Security Misconfiguration](images/0xc0-risk-explanation.png)