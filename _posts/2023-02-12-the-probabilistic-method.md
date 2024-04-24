---
title: The Probabilistic Method
description: a nice problem
tags: math probability
description: 
---
<p><!-- wp:quote --></p>
<blockquote class="wp-block-quote"><p><!-- wp:paragraph --></p>
<p>Mathematical truth is immutable; it lies outside physical reality... This is our belief; this is our core motivating force.</p>
<p><!-- /wp:paragraph --><cite>Joel Spencer, author of The Probabilistic Method</cite></p></blockquote>
<p><!-- /wp:quote --></p>
<p><!-- wp:paragraph --></p>
<p>The following problem &amp; proof, at least for me, outline the beauty of the probabilistic method. The first idea behind this problem is almost always induction. However, TPM gives way to an immediate result.</p>
<p><!-- /wp:paragraph --></p>
<div class="prob">
<p><strong>Problem 1</strong>. <em>Let <span class="math inline"><em>v</em><sub>1</sub>, …<em>v</em><sub><em>n</em></sub></span> be unit vectors in <span class="math inline">ℝ<sup><em>d</em></sup>.</span> Prove that it is possible to assign weights <span class="math inline">ℰ<sub><em>i</em></sub> ∈ { ± 1}</span> such that the vector <span class="math inline">∑<sub><em>i</em></sub>ℰ<sub><em>i</em></sub><em>v</em><sub><em>i</em></sub></span> has Euclidean norm less than or equal to <span class="math inline">√n.</span></em></p>
</div>
<div class="prob"></div>
<div class="proof">
<p><em>Proof.</em> Fix <span class="math inline"><em>n</em></span> to be a nonnegative integer. Then, fix a set of <span class="math inline"><em>n</em></span> unit vectors <span class="math inline"><em>v</em><sub>1</sub>, …<em>v</em><sub><em>n</em></sub>.</span> Let <span class="math inline"><em>W</em></span> be the random set of size <span class="math inline"><em>n</em></span> such that each element is either <span class="math inline">1</span> or <span class="math inline"> − 1</span> with equal probability <span class="math inline">1/2</span>. Denote the <span class="math inline"><em>i</em></span>th value of <span class="math inline"><em>W</em></span> as <span class="math inline">ℰ<sub><em>i</em></sub>.</span> Then, let <span class="math inline"><em>V</em></span> be <span class="math inline">∑<sub><em>i</em></sub>ℰ<sub><em>i</em></sub><em>v</em><sub><em>i</em></sub>,</span> e.g. the weighted sum of all the vectors. Then,</p>
</div>
<p class="has-text-align-center">
<div class="proof">
<p><span class="math display"><em>E</em>[|<em>V</em>|<sup>2</sup>] = <em>E</em>[(∑ℰ<sub><em>i</em></sub><em>v</em><sub><em>i</em></sub>)(∑ℰ<sub><em>i</em></sub><em>v</em><sub><em>i</em></sub>)] = ∑<sub><em>i</em></sub>∑<sub><em>j</em></sub><em>E</em>[ℰ<sub><em>i</em></sub>ℰ<sub><em>j</em></sub>]<em>v</em><sub><em>i</em></sub><em>v</em><sub><em>j</em></sub>.</span></p>
</div>
<div class="proof">
<p>Note that <span class="math inline"><em>E</em>[ℰ<sub><em>i</em></sub>ℰ<sub><em>j</em></sub>] = 0</span> if <span class="math inline"><em>i</em> ≠ <em>j</em></span>. If <span class="math inline"><em>i</em> = <em>j</em></span>, then <span class="math inline"><em>E</em>[ℰ<sub><em>i</em></sub><sup>2</sup>] = 1.</span> So, <span class="math display">∑<sub><em>i</em></sub>∑<sub><em>j</em></sub><em>E</em>[ℰ<sub><em>i</em></sub>ℰ<sub><em>j</em></sub>]<em>v</em><sub><em>i</em></sub><em>v</em><sub><em>j</em></sub> = ∑<sub><em>i</em></sub><em>v</em><sub><em>i</em></sub> ⋅ <em>v</em><sub><em>i</em></sub> = <em>n</em>.</span> </p>
</div>
<div class="proof">
<p>This means that there is a set of weights such that <span class="math inline">|<em>V</em>|<sup>2</sup> ≤ <em>n</em></span>. So, for this set of weights, <span class="math inline">|<em>V</em>| ≤ √n</span>. ◻</p>
</div>
