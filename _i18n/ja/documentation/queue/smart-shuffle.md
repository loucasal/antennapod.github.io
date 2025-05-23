スマートシャッフルは、高度なキューの並べ替え基準です。これを使用すると、できるだけキュー内に単一の購読のエピソードのクラスターができないようにしながら、公開日によってキューを並べ替えられます。

スマートシャッフルを使用するには、さまざまな購読からいくつかのエピソードをキューに入れ、上部バーの`…`をタップし、`並べ替え`を選択して、最後に`スマートシャッフル`を選択します。他の並べ替え基準と同様に、スマート シャッフルは昇順または降順で並べ替えられます。

## 詳しい仕組み

たとえばキューに15個のエピソードがあるとします。ポッドキャストA、B、Cからそれぞれ1個、ポッドキャストDから2個、ポッドキャストEから 10 個です。スマートシャッフルは、まずエピソードが最も多いポッドキャスト（E）を取得し、そのエピソードを次のように展開します。キュー: EE_EE_E_E_EE_EE。次に、2 番目に多いエピソードを含むポッドキャスト（D）を取得し、それらを使用可能なスロットEE_EEDE_EDEE_EEに振り分けます。これを、EEBEEDECEDEEAEEのようなキューが完成するまで続けます。

公開日は、ポッドキャスト*内*（この例では、ポッドキャストEのエピソードがそれに応じて並べ替えられます）とポッドキャスト*間*の両方で役割を果たします（ポッドキャストBのエピソードは、ポッドキャストAのエピソードよりも早いスポットを獲得します。前者の方が新しいためです）。
