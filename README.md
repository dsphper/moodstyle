
moodstyle机器学习脚本库
=======================




+ AdBoost.py
    + [BoostClassifier(object)](moodstyle/AdBoost.py#L6)
        + [__init__(self, classifier, weight=None)](moodstyle/AdBoost.py#L8)
        + [__call__(self, data)](moodstyle/AdBoost.py#L15)
        + [__str__(self)](moodstyle/AdBoost.py#L18)
    + [BoostData(object)](moodstyle/AdBoost.py#L22)
        + [__init__(self, data, weight=None)](moodstyle/AdBoost.py#L24)
    + [AdBoost(object)](moodstyle/AdBoost.py#L32)
        + [__init__(self, classifiers=\[\])](moodstyle/AdBoost.py#L34)
        + [train(self, datas)](moodstyle/AdBoost.py#L39)
        + [classify(self, data)](moodstyle/AdBoost.py#L59)
        + [__update_data_weight(self, trains, classifier)](moodstyle/AdBoost.py#L64)
        + [__str__(self)](moodstyle/AdBoost.py#L77)
        + [__get_trainer(self, trains)](moodstyle/AdBoost.py#L85)
+ AdTree.py
    + [Classifier(object)](moodstyle/AdTree.py#L7)
        + [__init__(self, classifier)](moodstyle/AdTree.py#L9)
        + [clear(self)](moodstyle/AdTree.py#L18)
        + [update_fit_value(self, data, value)](moodstyle/AdTree.py#L22)
        + [updates_fit_values(self, datas, values)](moodstyle/AdTree.py#L27)
        + [sync(self)](moodstyle/AdTree.py#L31)
        + [classify(self, data)](moodstyle/AdTree.py#L38)
        + [__str__(self)](moodstyle/AdTree.py#L43)
    + [AdTree(object)](moodstyle/AdTree.py#L51)
        + [__init__(self)](moodstyle/AdTree.py#L53)
        + [train(self, datas, weights, classifiers, diff=0.2)](moodstyle/AdTree.py#L57)
        + [find_min_loss(self, datas, residuals, classifiers)](moodstyle/AdTree.py#L85)
        + [update_residual(self, datas, residuals , classifier)](moodstyle/AdTree.py#L106)
        + [classify(self, data)](moodstyle/AdTree.py#L116)
+ Ann.py
    + [Ann(testInterface.Classify)](moodstyle/Ann.py#L17)
        + [__init__(self , w , learn_rate = 0.1 , labels = \[1 , -1 \])](moodstyle/Ann.py#L21)
        + [__train(self , data , label)](moodstyle/Ann.py#L29)
        + [classify(self , data , *argv , **kw )](moodstyle/Ann.py#L39)
        + [train(self , datas , labels , *argv , **kw)](moodstyle/Ann.py#L55)
+ Array.py
    + [PoolArray(objects)](moodstyle/Array.py#L12)
        + [__init__(self , objects , sample_rate )](moodstyle/Array.py#L15)
        + [create_rand_list(self)](moodstyle/Array.py#L24)
        + [next(self)](moodstyle/Array.py#L37)
    + [WaterSample(object)](moodstyle/Array.py#L45)
        + [__init__(self , objects , sample_rate)](moodstyle/Array.py#L48)
        + [get_rand_score(self )](moodstyle/Array.py#L55)
        + [next(self)](moodstyle/Array.py#L58)
    + [SampleArray(object)](moodstyle/Array.py#L73)
        + [__init__(self , objects , sample_    + = WaterSample)](moodstyle/Array.py#L76)
        + [__iter__(self)](moodstyle/Array.py#L84)
        + [__getitem__(self , index )](moodstyle/Array.py#L90)
+ Bandit.py
    + [Greedy(object)](moodstyle/Bandit.py#L8)
        + [__init__(self,e,N)](moodstyle/Bandit.py#L12)
        + [_prop(self)](moodstyle/Bandit.py#L23)
        + [getIndex(self)](moodstyle/Bandit.py#L32)
        + [process(self,label)](moodstyle/Bandit.py#L45)
    + [UCB(object)](moodstyle/Bandit.py#L53)
        + [__init__(self,N,max_value)](moodstyle/Bandit.py#L56)
        + [_prop(self)](moodstyle/Bandit.py#L66)
        + [getIndex(self)](moodstyle/Bandit.py#L72)
        + [process(self,label)](moodstyle/Bandit.py#L80)
+ BaseStrut.py
    + [WeightArray(object)](moodstyle/BaseStrut.py#L5)
        + [__init__(self, datas, distance_fun)](moodstyle/BaseStrut.py#L8)
        + [__getitem__(self, label_tuple)](moodstyle/BaseStrut.py#L22)
        + [get_distance_by_index(self  , row , line )](moodstyle/BaseStrut.py#L32)
        + [create_distance_map(self, datas, distance_fun)](moodstyle/BaseStrut.py#L46)
    + [Normalization(object)](moodstyle/BaseStrut.py#L72)
	    + [__init__(self, *argv , **kw)](moodstyle/BaseStrut.py#L75)
	    + [update(self , value)](moodstyle/BaseStrut.py#L79)
	    + [get_normalization(self ,value )](moodstyle/BaseStrut.py#L83)
    + [MinMax(Normalization)](moodstyle/BaseStrut.py#L88)
	    + [__init__(self , max_value = None , min_value = None ) ](moodstyle/BaseStrut.py#L95)
	    + [update(self , value)](moodstyle/BaseStrut.py#L107)
	    + [get_normalization(self , value )](moodstyle/BaseStrut.py#L129)
    + [ZScore(Normalization)](moodstyle/BaseStrut.py#L148)
	    + [__init__(self)](moodstyle/BaseStrut.py#L153)
	    + [update(self , values)](moodstyle/BaseStrut.py#L159)
	    + [get_normalization(self , value)](moodstyle/BaseStrut.py#L168)
    + [LogNormalization(Normalization)](moodstyle/BaseStrut.py#L176)
	    + [__init__(self , base = 10 )](moodstyle/BaseStrut.py#L179)
	    + [get_normalization(self , value )](moodstyle/BaseStrut.py#L193)
    + [Arccotx(Normalization)](moodstyle/BaseStrut.py#L198)
	    + [get_normalization(self , value )](moodstyle/BaseStrut.py#L201)
+ Bayes.py
    + [Bayes(object)](moodstyle/Bayes.py#L7)
        + [train(self, datas, attr_len, labels, dense=True)](moodstyle/Bayes.py#L10)
        + [_predict(self , data , label)](moodstyle/Bayes.py#L45)
        + [get_prob(self , attr_index , value ,label )](moodstyle/Bayes.py#L53)
        + [predict(self, data)](moodstyle/Bayes.py#L71)
        + [predict_old(self, data)](moodstyle/Bayes.py#L83)
+ Bp.py
    + [Layer(object)](moodstyle/Bp.py#L12)
        + [__init__(self , layer_count , default = 1.)](moodstyle/Bp.py#L15)
        + [__len__(self)](moodstyle/Bp.py#L19)
    + [RatioArray(object)](moodstyle/Bp.py#L22)
        + [__init__(self, line , row , min_value , max_value )](moodstyle/Bp.py#L25)
    + [Bp(object)](moodstyle/Bp.py#L36)
    + [rand(a, b)](moodstyle/Bp.py#L54)
    + [makeMatrix(I, J, fill=0.0)](moodstyle/Bp.py#L58)
    + [sigmoid(x)](moodstyle/Bp.py#L65)
    + [dsigmoid(y)](moodstyle/Bp.py#L70)
    + [NN](moodstyle/Bp.py#L73)
        + [__init__(self, ni, nh, no)](moodstyle/Bp.py#L75)
        + [update(self, inputs)](moodstyle/Bp.py#L101)
        + [backPropagate(self, targets, N, M)](moodstyle/Bp.py#L126)
        + [test(self, patterns)](moodstyle/Bp.py#L166)
        + [weights(self)](moodstyle/Bp.py#L170)
        + [train(self, patterns, iterations=1000, N=0.5, M=0.1)](moodstyle/Bp.py#L179)
    + [demo()](moodstyle/Bp.py#L193)
+ Bp1.py
    + [Neroun(object)](moodstyle/Bp1.py#L7)
        + [__init__(self , weight_len , learn_rate = 0.1 , delta = random.uniform(1 , -1))](moodstyle/Bp1.py#L10)
        + [init_weights(self , weight_len  , weight_max = 0.5 , weight_min = -0.5)](moodstyle/Bp1.py#L17)
        + [predict(self , inputs)](moodstyle/Bp1.py#L20)
        + [simgod(self , value)](moodstyle/Bp1.py#L23)
        + [disgod(self , target)](moodstyle/Bp1.py#L26)
        + [__len__(self)](moodstyle/Bp1.py#L29)
        + [__getitem__(self , index)](moodstyle/Bp1.py#L32)
        + [__setitem__(self , index , value)](moodstyle/Bp1.py#L35)
        + [update(self , target, predict)](moodstyle/Bp1.py#L38)
    + [Layer(object)](moodstyle/Bp1.py#L44)
        + [__init__(self , inputs_len ,neroun_len , learn_rate = 0.1)](moodstyle/Bp1.py#L48)
        + [predict(self , inputs )](moodstyle/Bp1.py#L64)
        + [train_predict(self , inputs)](moodstyle/Bp1.py#L67)
        + [update(self , deltas)](moodstyle/Bp1.py#L72)
        + [get_delta(self ,errors)](moodstyle/Bp1.py#L77)
    + [OutPutLayer(Layer)](moodstyle/Bp1.py#L80)
        + [get_delta(self , errors )](moodstyle/Bp1.py#L82)
    + [HiddenLayer(Layer)](moodstyle/Bp1.py#L85)
        + [__init__(self , inputs_len ,neroun_len  , next_layer, learn_rate = 0.1)](moodstyle/Bp1.py#L87)
        + [get_delta(self , errors )](moodstyle/Bp1.py#L91)
    + [Bp(object)](moodstyle/Bp1.py#L98)
        + [__init__(self , inputs_len , hidden_len , outputs_len)](moodstyle/Bp1.py#L102)
        + [predict(self , inputs)](moodstyle/Bp1.py#L110)
        + [_train_predict(self , inputs)](moodstyle/Bp1.py#L117)
        + [train(self , inputs ,targets )](moodstyle/Bp1.py#L125)
+ Canopy.py
    + [Canopy(object)](moodstyle/Canopy.py#L7)
        + [__init__(self, centre)](moodstyle/Canopy.py#L13)
        + [__str__(self)](moodstyle/Canopy.py#L17)
    + [CanopyCluster(object)](moodstyle/Canopy.py#L22)
        + [__init__(self, t1, t2)](moodstyle/Canopy.py#L44)
        + [cluster(self, datas)](moodstyle/Canopy.py#L50)
        + [distance(self, data1, data2)](moodstyle/Canopy.py#L75)
    + [SimpleCanopyCluster(CanopyCluster)](moodstyle/Canopy.py#L79)
        + [distance(self, data1, data2)](moodstyle/Canopy.py#L81)
+ Cart.py
    + [Node(object)](moodstyle/Cart.py#L10)
        + [__init__(self, split_attr, split_value)](moodstyle/Cart.py#L12)
        + [__str__(self)](moodstyle/Cart.py#L18)
    + [CartTree(object)](moodstyle/Cart.py#L22)
        + [__init__(self)](moodstyle/Cart.py#L24)
        + [load_model(self, file_path)](moodstyle/Cart.py#L28)
        + [save(self, model_path)](moodstyle/Cart.py#L37)
        + [__train(self, datas, labels, attrs, threshold=0.01)](moodstyle/Cart.py#L43)
        + [split_data_by_attr(self, datas, attrs, attr_name)](moodstyle/Cart.py#L70)
        + [train(self, datas, attrs, labels, threshold=0.01)](moodstyle/Cart.py#L87)
        + [get_split_attr(self, attrs, attr)](moodstyle/Cart.py#L92)
        + [get_split_value(self, datas, split_index)](moodstyle/Cart.py#L99)
        + [calc_gini(self, datas, labels, split_index, split_value)](moodstyle/Cart.py#L107)
        + [get_best_feature(self, datas, labels, attrs)](moodstyle/Cart.py#L137)
        + [_classify(self, data, attrs, node)](moodstyle/Cart.py#L169)
        + [classify(self, data)](moodstyle/Cart.py#L180)
+ DDistance.py
    + [DDdistance(object)](moodstyle/DDistance.py#L6)
        + [distance(self, data1, data2)](moodstyle/DDistance.py#L8)
    + [Manhattan(DDdistance)](moodstyle/DDistance.py#L12)
        + [distance(self, data1, data2)](moodstyle/DDistance.py#L18)
    + [DefaultDistance(DDdistance)](moodstyle/DDistance.py#L24)
        + [distance(self, data1, data2)](moodstyle/DDistance.py#L26)
    + [Chebyshev(DDdistance)](moodstyle/DDistance.py#L35)
        + [distance(self, data1, data2)](moodstyle/DDistance.py#L41)
    + [Cosine(DDdistance)](moodstyle/DDistance.py#L47)
        + [distance(self, data1, data2)](moodstyle/DDistance.py#L53)
    + [Hamming(DDdistance)](moodstyle/DDistance.py#L63)
        + [distance(self, data1, data2)](moodstyle/DDistance.py#L69)
    + [Euclidean(DDdistance)](moodstyle/DDistance.py#L73)
        + [distance(self, data1, data2)](moodstyle/DDistance.py#L79)
+ DataSet.py
    + [DList(list)](moodstyle/DataSet.py#L6)
        + [items(self)](moodstyle/DataSet.py#L8)
        + [has_key(self , value)](moodstyle/DataSet.py#L11)
        + [update(self , data)](moodstyle/DataSet.py#L19)
        + [keys(self)](moodstyle/DataSet.py#L31)
        + [order_key(self)](moodstyle/DataSet.py#L34)
        + [values(self)](moodstyle/DataSet.py#L37)
    + [DeseData(DList)](moodstyle/DataSet.py#L42)
        + [__init__(self , data  ,  default_value  ,  data_len  , *argv , **kw)](moodstyle/DataSet.py#L46)
        + [__len__(self)](moodstyle/DataSet.py#L59)
        + [__setitem__(self , index , value )](moodstyle/DataSet.py#L62)
    + [SparseData(dict)](moodstyle/DataSet.py#L68)
        + [__init__(self ,data , default_value , data_len , *argv , **kw)](moodstyle/DataSet.py#L72)
        + [__getitem__(self , index )](moodstyle/DataSet.py#L79)
        + [__setitem__(self , index , value)](moodstyle/DataSet.py#L82)
        + [__len__(self)](moodstyle/DataSet.py#L91)
        + [order_key(self)](moodstyle/DataSet.py#L94)
    + [DataSet(DList)](moodstyle/DataSet.py#L97)
        + [__init__(self ,data_len, dense_data , *argv , **kw)](moodstyle/DataSet.py#L101)
        + [append(self , data = None)](moodstyle/DataSet.py#L117)
        + [extend(self , data)](moodstyle/DataSet.py#L132)
        + [shape(self)](moodstyle/DataSet.py#L144)
        + [data_range(self)](moodstyle/DataSet.py#L147)
+ DbScan.py
    + [ClusterItem(object)](moodstyle/DbScan.py#L5)
        + [__init__(self , data)](moodstyle/DbScan.py#L8)
    + [DbScan(object)](moodstyle/DbScan.py#L15)
        + [cluster(self , datas , radius , minPoint)](moodstyle/DbScan.py#L18)
        + [distance(self , data1  , data2 )](moodstyle/DbScan.py#L66)
+ DecisionTree.py
    + [Node(object)](moodstyle/DecisionTree.py#L9)
        + [__init__(self, attr_name=None, label=None)](moodstyle/DecisionTree.py#L11)
        + [__str__(self)](moodstyle/DecisionTree.py#L16)
    + [DecisionTree(object)](moodstyle/DecisionTree.py#L23)
        + [__init__(self)](moodstyle/DecisionTree.py#L25)
        + [train(self, datas, attrs, threshold=0.01, denseData=True, tree=None)](moodstyle/DecisionTree.py#L29)
        + [entropy(probs)](moodstyle/DecisionTree.py#L65)
        + [getSplitAttrs(self, attrs, attr)](moodstyle/DecisionTree.py#L72)
        + [getBestFeature(self, datas, attrs, denseData)](moodstyle/DecisionTree.py#L79)
        + [splitDataByAttr(self, datas, attrs, attr_name, attr_value, denseData=True)](moodstyle/DecisionTree.py#L138)
        + [classify(self, data)](moodstyle/DecisionTree.py#L156)
+ DecisionTree1.py
    + [Node(dict)](moodstyle/DecisionTree1.py#L11)
    + [DecisionTree(object)](moodstyle/DecisionTree1.py#L15)
        + [__init__(self)](moodstyle/DecisionTree1.py#L17)
        + [load_model(self, file_path)](moodstyle/DecisionTree1.py#L21)
        + [save(self, model_path)](moodstyle/DecisionTree1.py#L30)
        + [__train(self, datas , labels , attrs, threshold=0.01, dense_data=True)](moodstyle/DecisionTree1.py#L36)
        + [train(self, datas , labels , attrs, threshold=0.01, dense_data=True)](moodstyle/DecisionTree1.py#L71)
        + [entropy(probs)](moodstyle/DecisionTree1.py#L76)
        + [get_split_attr(self, attrs, attr)](moodstyle/DecisionTree1.py#L83)
        + [get_best_feature(self, datas, labels, attrs, dense_data)](moodstyle/DecisionTree1.py#L90)
        + [split_data_by_attr(self, datas , labels , attrs, attr_name, attr_value, dense_data=True)](moodstyle/DecisionTree1.py#L93)
        + [classify(self, data)](moodstyle/DecisionTree1.py#L114)
    + [ID3(DecisionTree)](moodstyle/DecisionTree1.py#L137)
        + [get_best_feature(self, datas , labels , attrs, dense_data)](moodstyle/DecisionTree1.py#L139)
    + [C45(ID3)](moodstyle/DecisionTree1.py#L198)
        + [get_best_feature(self, datas , labels, attrs, dense_data)](moodstyle/DecisionTree1.py#L200)
+ DefaultValue.py
    + [MissingValue(object)](moodstyle/DefaultValue.py#L4)
        + [get_value(self, feature)](moodstyle/DefaultValue.py#L6)
    + [ArvgMissingValue(object)](moodstyle/DefaultValue.py#L10)
        + [__init__(self, feature_len)](moodstyle/DefaultValue.py#L12)
        + [add(self, feature, value)](moodstyle/DefaultValue.py#L15)
+ Dict.py
    + [Dictionary(dict)](moodstyle/Dict.py#L9)
        + [__init__(self , **kw)](moodstyle/Dict.py#L11)
        + [open_dict(self , dict_path)](moodstyle/Dict.py#L17)
        + [__setitem__(self ,key, value)](moodstyle/Dict.py#L22)
        + [to_vector(self , words)](moodstyle/Dict.py#L29)
        + [to_one_hot(self , words)](moodstyle/Dict.py#L37)
+ Emm.py
    + [Emm(object)](moodstyle/Emm.py#L9)
        + [__init__(self )](moodstyle/Emm.py#L13)
+ Feature.py
    + [Binning(object)](moodstyle/Feature.py#L8)
        + [__init__(self,k,box = None)](moodstyle/Feature.py#L12)
        + [train(self,features)](moodstyle/Feature.py#L22)
        + [predict(self,feature)](moodstyle/Feature.py#L26)
        + [_sort(self,array)](moodstyle/Feature.py#L32)
    + [EqualRate(Binning)](moodstyle/Feature.py#L37)
        + [train(self,features)](moodstyle/Feature.py#L40)
    + [EqualLength(Binning)](moodstyle/Feature.py#L45)
        + [train(self,features)](moodstyle/Feature.py#L56)
+ FeatureExtract.py
    + [Document(object)](moodstyle/FeatureExtract.py#L6)
        + [__init__(self)](moodstyle/FeatureExtract.py#L11)
        + [insert_document(self, doc_type, document= \[\])](moodstyle/FeatureExtract.py#L16)
        + [get_word_count(self, word)](moodstyle/FeatureExtract.py#L37)
        + [get_type_word_count(self, doc_type, word)](moodstyle/FeatureExtract.py#L51)
        + [get_doc_count(self, doc_type)](moodstyle/FeatureExtract.py#L62)
        + [get_word_set(self)](moodstyle/FeatureExtract.py#L72)
        + [get_type_set(self)](moodstyle/FeatureExtract.py#L81)
        + [__str__(self)](moodstyle/FeatureExtract.py#L92)
    + [ITextFeatureScore(object)](moodstyle/FeatureExtract.py#L95)
        + [feature_socre(self, doc_word_count, doc_count, word_count, doc_sum)](moodstyle/FeatureExtract.py#L98)
    + [CreateDocument(object)](moodstyle/FeatureExtract.py#L116)
        + [__init__(self)](moodstyle/FeatureExtract.py#L118)
        + [insert_document_list(self, doc_name, contents, ngram=1, word_split=' ')](moodstyle/FeatureExtract.py#L121)
        + [text_extract(self, words , ngram = 2,  word_split = None)](moodstyle/FeatureExtract.py#L145)
    + [TextFeature(object)](moodstyle/FeatureExtract.py#L154)
        + [__init__(self, min_word_count=0, filter_rate=0.003)](moodstyle/FeatureExtract.py#L156)
        + [extract_feature(self, doc, top_word=0.01)](moodstyle/FeatureExtract.py#L160)
        + [text_feature_score(self, doc_word_count, doc_count, word_count, doc_sum)](moodstyle/FeatureExtract.py#L189)
        + [filter(self, doc , doc_type , word)](moodstyle/FeatureExtract.py#L200)
    + [IM(TextFeature)](moodstyle/FeatureExtract.py#L205)
        + [text_feature_score(self, doc_word_count, doc_count, word_count, doc_sum)](moodstyle/FeatureExtract.py#L212)
    + [CHI(TextFeature)](moodstyle/FeatureExtract.py#L216)
        + [text_feature_score(self, doc_word_count, doc_count, word_count, doc_sum)](moodstyle/FeatureExtract.py#L218)
    + [DF(TextFeature)](moodstyle/FeatureExtract.py#L226)
        + [text_feature_score(self, doc_word_count, doc_count, word_count, doc_sum)](moodstyle/FeatureExtract.py#L234)
    + [WLLR(TextFeature)](moodstyle/FeatureExtract.py#L241)
        + [text_feature_score(self, doc_word_count, doc_count, word_count, doc_sum)](moodstyle/FeatureExtract.py#L243)
    + [IG(TextFeature)](moodstyle/FeatureExtract.py#L254)
+ GRTree.py
+ HCluster.py
    + [HierarchicalClustering(object)](moodstyle/HCluster.py#L9)
        + [__init__(self)](moodstyle/HCluster.py#L11)
        + [cluster(self, datas, cluster_num,  threshold=0.03)](moodstyle/HCluster.py#L14)
        + [distance(self, data1, data2)](moodstyle/HCluster.py#L45)
        + [get_cluster_distance(self, cluster1, cluster2, distance_map)](moodstyle/HCluster.py#L58)
    + [ALHierarchicalClustering(HierarchicalClustering)](moodstyle/HCluster.py#L72)
        + [get_cluster_distance(self, cluster1, cluster2, distance_map)](moodstyle/HCluster.py#L77)
    + [SLHierarchicalClustering(HierarchicalClustering)](moodstyle/HCluster.py#L81)
        + [get_cluster_distance(self, cluster1, cluster2, distance_map)](moodstyle/HCluster.py#L87)
    + [CLHierarchicalClustering(HierarchicalClustering)](moodstyle/HCluster.py#L92)
        + [get_cluster_distance(self, cluster1, cluster2, distance_map)](moodstyle/HCluster.py#L98)
+ Hmm.py
    + [HmmItem(object)](moodstyle/Hmm.py#L12)
        + [__init__(self, obs, hide)](moodstyle/Hmm.py#L16)
        + [__str__(self)](moodstyle/Hmm.py#L20)
    + [HmmItems(list)](moodstyle/Hmm.py#L24)
        + [__check(self, value)](moodstyle/Hmm.py#L33)
        + [__setitem__(self, key, value)](moodstyle/Hmm.py#L37)
        + [append(self, value)](moodstyle/Hmm.py#L46)
        + [__str__(self)](moodstyle/Hmm.py#L55)
    + [HmmModel(object)](moodstyle/Hmm.py#L58)
        + [__init__(self, states)](moodstyle/Hmm.py#L60)
        + [create_start_states(self, states, init_value=0.)](moodstyle/Hmm.py#L70)
        + [create_transition_probability(self, states, init_value=0.)](moodstyle/Hmm.py#L76)
        + [create_emission_probability(self, states)](moodstyle/Hmm.py#L84)
    + [Hmm(object)](moodstyle/Hmm.py#L93)
        + [__init__(self, model_path)](moodstyle/Hmm.py#L95)
        + [load(self, model_path)](moodstyle/Hmm.py#L102)
        + [viterbi(self, obs)](moodstyle/Hmm.py#L106)
    + [TrainHmm(object)](moodstyle/Hmm.py#L130)
        + [__init__(self, states)](moodstyle/Hmm.py#L132)
        + [save(self, model_path)](moodstyle/Hmm.py#L135)
        + [add_items(self, hmmitems)](moodstyle/Hmm.py#L139)
        + [translate(self)](moodstyle/Hmm.py#L157)
    + [TrainSeg(object)](moodstyle/Hmm.py#L182)
        + [__init__(self , states = \['s' , 'e' , 'm' ,'b'\])](moodstyle/Hmm.py#L184)
        + [add_line(self , line)](moodstyle/Hmm.py#L188)
        + [word_state(self , word)](moodstyle/Hmm.py#L198)
        + [train()](moodstyle/Hmm.py#L212)
+ Hmm1.py
    + [HmmItem(object)](moodstyle/Hmm1.py#L12)
        + [__init__(self, obs, hide)](moodstyle/Hmm1.py#L16)
        + [__str__(self)](moodstyle/Hmm1.py#L20)
    + [HmmItems(list)](moodstyle/Hmm1.py#L24)
        + [__check(self, value)](moodstyle/Hmm1.py#L33)
        + [__setitem__(self, key, value)](moodstyle/Hmm1.py#L37)
        + [append(self, value)](moodstyle/Hmm1.py#L46)
        + [__str__(self)](moodstyle/Hmm1.py#L55)
    + [HmmModel(object)](moodstyle/Hmm1.py#L58)
        + [__init__(self, states)](moodstyle/Hmm1.py#L60)
        + [create_start_states(self, states, init_value=0.)](moodstyle/Hmm1.py#L70)
        + [create_transition_probability(self, states, init_value=0.)](moodstyle/Hmm1.py#L76)
        + [create_emission_probability(self, states)](moodstyle/Hmm1.py#L84)
    + [Hmm(object)](moodstyle/Hmm1.py#L93)
        + [__init__(self, model_path)](moodstyle/Hmm1.py#L95)
        + [load(self, model_path)](moodstyle/Hmm1.py#L102)
        + [viterbi(self, obs)](moodstyle/Hmm1.py#L106)
    + [TrainHmm(object)](moodstyle/Hmm1.py#L130)
        + [__init__(self, states)](moodstyle/Hmm1.py#L132)
        + [save(self, model_path)](moodstyle/Hmm1.py#L135)
        + [add_items(self, hmmitems)](moodstyle/Hmm1.py#L139)
        + [translate(self)](moodstyle/Hmm1.py#L157)
    + [TrainSeg(object)](moodstyle/Hmm1.py#L182)
        + [__init__(self , states = \['s' , 'e' , 'm' ,'b'\])](moodstyle/Hmm1.py#L184)
        + [add_line(self , line)](moodstyle/Hmm1.py#L188)
        + [word_state(self , word)](moodstyle/Hmm1.py#L198)
+ Interface.py
    + [Classify(object)](moodstyle/Interface.py#L7)
        + [classify(self , data , *argv , **kw)](moodstyle/Interface.py#L12)
    + [Regression(object)](moodstyle/Interface.py#L16)
        + [predict(self , data , *argv , **kw)](moodstyle/Interface.py#L21)
+ KdTree.py
+ Kmeans.py
    + [Center(object)](moodstyle/Kmeans.py#L24)
        + [__init__(self, label, center_vector, distance_fun=None)](moodstyle/Kmeans.py#L26)
        + [__sub__(self, value)](moodstyle/Kmeans.py#L38)
    + [Kmeans(object)](moodstyle/Kmeans.py#L52)
        + [cluster(self, datas, k, iter_count=10000, diff=0.00001)](moodstyle/Kmeans.py#L54)
        + [rand_seed(self, datas, k)](moodstyle/Kmeans.py#L89)
        + [update_centers(self, datas, labels, centers)](moodstyle/Kmeans.py#L94)
    + [DKmeans(Kmeans)](moodstyle/Kmeans.py#L107)
        + [distance(self, data1, data2)](moodstyle/Kmeans.py#L109)
    + [ManhattanKmeans(Kmeans, Manhattan)](moodstyle/Kmeans.py#L118)
    + [HammingKmeans(Kmeans, Hamming)](moodstyle/Kmeans.py#L123)
    + [CosineKmeans(Kmeans, Cosine)](moodstyle/Kmeans.py#L128)
    + [EuclideanKmeans(Kmeans, Euclidean)](moodstyle/Kmeans.py#L132)
+ KmeansPlusPlus.py
    + [KmeansPlusPlus(Kmeans)](moodstyle/KmeansPlusPlus.py#L10)
        + [rand_seed(self, datas, k)](moodstyle/KmeansPlusPlus.py#L12)
    + [DKmeansPlusPlus(KmeansPlusPlus , DKmeans)](moodstyle/KmeansPlusPlus.py#L40)
+ Knn.py
    + [ClassItem(object)](moodstyle/Knn.py#L4)
    + [KdNode(object)](moodstyle/Knn.py#L9)
        + [__init__(self, split, left_child, right_child, data, parrent_node)](moodstyle/Knn.py#L11)
    + [KdTree(object)](moodstyle/Knn.py#L19)
        + [create_kd_tree(self, datas, k, feature_len, depth)](moodstyle/Knn.py#L21)
        + [get_split_index(self, datas, k, feature_len, depth)](moodstyle/Knn.py#L30)
    + [Knn(object)](moodstyle/Knn.py#L48)
        + [__init__(self, train_data, labels, top_n)](moodstyle/Knn.py#L50)
        + [classify(self, data)](moodstyle/Knn.py#L55)
+ LinerModel.py
    + [LinerModel(object)](moodstyle/LinerModel.py#L6)
        + [train(self , datas , labels , item_len , learn_rate )](moodstyle/LinerModel.py#L12)
        + [update_weight(self , l , target , data , learn_rate)](moodstyle/LinerModel.py#L21)
        + [predict(self , data)](moodstyle/LinerModel.py#L28)
+ Logistic.py
    + [Logistic(object)](moodstyle/Logistic.py#L6)
        + [train(self, datas, labels, alpha=0.001)](moodstyle/Logistic.py#L8)
        + [classify(self, data)](moodstyle/Logistic.py#L19)
        + [sigmod(self, x)](moodstyle/Logistic.py#L24)
+ MiniBatchKMeans.py
    + [MiniBatchKmeans(Kmeans)](moodstyle/MiniBatchKMeans.py#L17)
        + [cluster(self, datas, k, iter_count=10000, diff=0.00001)](moodstyle/MiniBatchKMeans.py#L19)
        + [rand_seed(self, datas, k)](moodstyle/MiniBatchKMeans.py#L60)
        + [add(self, center, data, eta, data_len)](moodstyle/MiniBatchKMeans.py#L63)
    + [DMiniBatchKmeans(MiniBatchKmeans, DefaultDistance)](moodstyle/MiniBatchKMeans.py#L69)
+ Ngram.py
    + [ngram(content, splitor = " "  , n = 2 )](moodstyle/Ngram.py#L7)
+ OneHotCode.py
    + [OneHotCode(object)](moodstyle/OneHotCode.py#L9)
        + [__init__(self)](moodstyle/OneHotCode.py#L25)
        + [train(self,data)](moodstyle/OneHotCode.py#L28)
        + [predict(self,data)](moodstyle/OneHotCode.py#L33)
+ PageRank.py
    + [Graph(object)](moodstyle/PageRank.py#L11)
        + [__init__(self , point_len , dense = True )](moodstyle/PageRank.py#L14)
        + [__len__(self)](moodstyle/PageRank.py#L24)
        + [add_edge(self , point_a , point_b)](moodstyle/PageRank.py#L27)
        + [keys(self)](moodstyle/PageRank.py#L37)
        + [ins(self , point)](moodstyle/PageRank.py#L40)
        + [outs(self , point)](moodstyle/PageRank.py#L43)
        + [outs_count(self , point)](moodstyle/PageRank.py#L49)
        + [update(self,weights)](moodstyle/PageRank.py#L52)
    + [GraphV2(object)](moodstyle/PageRank.py#L61)
        + [__init__(self,point_len)](moodstyle/PageRank.py#L65)
        + [__len__(self)](moodstyle/PageRank.py#L72)
        + [add_edge(self ,point_a , point_b)](moodstyle/PageRank.py#L75)
        + [keys(self)](moodstyle/PageRank.py#L79)
        + [outs_count(self,point)](moodstyle/PageRank.py#L82)
        + [update(self,weights)](moodstyle/PageRank.py#L85)
        + [ins(self,point)](moodstyle/PageRank.py#L93)
    + [PageRank(object)](moodstyle/PageRank.py#L96)
        + [rank(self , graph ,iter_count = 1000, d = 0.85 , min_error = 0.01)](moodstyle/PageRank.py#L99)
        + [calc_error(self , weights , graph)](moodstyle/PageRank.py#L111)
+ RandomForst.py
    + [RF(object)](moodstyle/RandomForst.py#L6)
+ RegressionTree.py
    + [TreeNode(object)](moodstyle/RegressionTree.py#L5)
        + [__init__(self)](moodstyle/RegressionTree.py#L9)
    + [RegressionTree(object)](moodstyle/RegressionTree.py#L15)
        + [__init__(self)](moodstyle/RegressionTree.py#L20)
        + [train(self , datasets , targets)](moodstyle/RegressionTree.py#L26)
        + [loss(self , datasets , labels , attr , split_value)](moodstyle/RegressionTree.py#L30)
        + [get_target_avg(self , datasets ,targets , attr , split_value)](moodstyle/RegressionTree.py#L55)
+ __init__.py
+ config.py
    + [set_prefs(prefs)](moodstyle/config.py#L4)
    + [project_opened(project)](moodstyle/config.py#L94)
