


irl  from  demo






Visual Reinforcement Learning with Imagined Goals
Ashvin Nair⇤
, Vitchyr Pong⇤, Murtaza Dalal, Shikhar Bahl, Steven Lin, Sergey Levine
University of California, Berkeley
{anair17,vitchyr,mdalal,shikharbahl,stevenlin598,svlevine}@berkeley.edu
Abstract
For an autonomous agent to fulfill a wide range of user-specified goals at test time,
it must be able to learn broadly applicable and general-purpose skill repertoires.
Furthermore, to provide the requisite level of generality, these skills must handle
raw sensory input such as images. In this paper, we propose an algorithm that
acquires such general-purpose skills by combining unsupervised representation
learning and reinforcement learning of goal-conditioned policies. Since the particular goals that might be required at test-time are not known in advance, the agent
performs a self-supervised “practice” phase where it imagines goals and attempts
to achieve them. We learn a visual representation with three distinct purposes: sampling goals for self-supervised practice, providing a structured transformation of
raw sensory inputs, and computing a reward signal for goal reaching. We also propose a retroactive goal relabeling scheme to further improve the sample-efficiency
of our method. Our off-policy algorithm is efficient enough to learn policies that
operate on raw image observations and goals for a real-world robotic system, and
substantially outperforms prior techniques.


Visual reinforcement learning with imagined goals
[PDF] arxiv.org
Catastrophic Importance of Catastrophic Forgetting
A Ierusalem - arXiv preprint arXiv:1808.07049, 2018 - arxiv.org
This paper describes some of the possibilities of artificial neural networks that open up after 
solving the problem of catastrophic forgetting. A simple model and reinforcement learning 
applications of existing methods are also proposed. Subjects: Machine Learning (cs. LG); …
  All 3 versions 
[PDF] openreview.net
The Implicit Preference Information in an Initial State
R Shah, D Krasheninnikov, J Alexander, P Abbeel… - 2018 - openreview.net
Reinforcement learning (RL) agents optimize only the features specified in a reward function 
and are indifferent to anything left out inadvertently. This means that we must not only 
specify what to do, but also the much larger space of what not to do. It is easy to forget these …
  
[PDF] arxiv.org
Learning Actionable Representations with Goal-Conditioned Policies
D Ghosh, A Gupta, S Levine - arXiv preprint arXiv:1811.07819, 2018 - arxiv.org
Representation learning is a central challenge across a range of machine learning areas. In 
reinforcement learning, effective and functional representations have the potential to 
tremendously accelerate learning progress and solve more challenging problems. Most …
  All 4 versions 
[PDF] arxiv.org
Unsupervised Control Through Non-Parametric Discriminative Rewards
D Warde-Farley, T Van de Wiele, T Kulkarni… - arXiv preprint arXiv …, 2018 - arxiv.org
Learning to control an environment without hand-crafted rewards or expert data remains 
challenging and is at the frontier of reinforcement learning research. We present an 
unsupervised learning algorithm to train agents to achieve perceptually-specified goals …
  All 3 versions 
[PDF] arxiv.org
Self-supervised Learning of Image Embedding for Continuous Control
C Florensa, J Degrave, N Heess… - arXiv preprint arXiv …, 2019 - arxiv.org
Operating directly from raw high dimensional sensory inputs like images is still a challenge 
for robotic control. Recently, Reinforcement Learning methods have been proposed to solve 
specific tasks end-to-end, from pixels to torques. However, these approaches assume the …
  All 2 versions 
[PDF] arxiv.org
Variational Autoencoders Pursue PCA Directions (by Accident)










Algorithms for inverse reinforcement learning

https://www.researchgate.net/profile/Changxi_You/publication/330400231_Advanced_Planning_for_Autonomous_Vehicles_Using_Reinforcement_Learning_and_Deep_Inverse_Reinforcement_Learning/links/5c3e13b0299bf12be3c9f540/Advanced-Planning-for-Autonomous-Vehicles-Using-Reinforcement-Learning-and-Deep-Inverse-Reinforcement-Learning.pdf
Advanced Planning for Autonomous Vehicles Using Reinforcement
Learning and Deep Inverse Reinforcement Learning
Changxi You1
Jianbo Lu2 Dimitar Filev3 Panagiotis Tsiotras4
January 8, 2019
Abstract
Autonomous vehicles promise to improve traffic safety while, at the same time, increase fuel efficiency and reduce
congestion. They represent the main trend in future intelligent transportation systems. This paper concentrates on the
planning problem of autonomous vehicles in traffic. We model the interaction between the autonomous vehicle and
the environment as a stochastic Markov decision process (MDP) and consider the driving style of an expert driver as
the target to be learned. The road geometry is taken into consideration in the MDP model in order to incorporate more
diverse driving styles. The desired, expert-like driving behavior of the autonomous vehicle is obtained as follows: First,
we design the reward function of the corresponding MDP and determine the optimal driving strategy for the autonomous
vehicle using reinforcement learning techniques. Second, we collect a number of demonstrations from an expert driver
and learn the optimal driving strategy based on data using inverse reinforcement learning. The unknown reward function
of the expert driver is approximated using a deep neural-network (DNN). We clarify and validate the application of the
maximum entropy principle (MEP) to learn the DNN reward function, and provide the necessary derivations for using
the maximum entropy principle to learn a parameterized feature (reward) function. Simulated results demonstrate the
desired driving behaviors of an autonomous vehicle using both the reinforcement learning and inverse reinforcement
learning techniques.



VIREL:  还有 serge leven 几篇相关；
A Variational Inference Framework for
Reinforcement Learning
Matthew Fellows† Anuj Mahajan† Tim G. J. Rudner Shimon Whiteson
University of Oxford University of Oxford University of Oxford University of Oxford
Abstract
Applying probabilistic models to reinforcement
learning (RL) has become an exciting direction
of research owing to powerful optimisation tools
such as variational inference becoming applicable
to RL. However, due to their formulation, existing inference frameworks and their algorithms
pose significant challenges for learning optimal
policies, for example, the absence of mode capturing behaviour in pseudo-likelihood methods and
difficulties in optimisation of learning objective
in maximum entropy RL based approaches. We
propose VIREL, a novel, theoretically grounded
probabilistic inference framework for RL that
utilises the action-value function in a parametrised
form to capture future dynamics of the underlying
Markov decision process. Owing to its generality,
our framework lends itself to current advances
in variational inference. Applying the variational
expectation-maximisation algorithm to our framework, we show that the actor-critic algorithm can
be reduced to expectation-maximisation. We derive a family of methods from our framework,
including state-of-the-art methods based on soft
value functions. We evaluate two actor-critic algorithms derived from this family, which perform
on par with soft actor critic, demonstrating that
our framework of

1
We evaluate our simple algorithm
against an existing state of the art actor-critic algorithm,
soft actor-critic (SAC), demonstrating similar performance
across a variety of OpenAI gym domains (Brockman et al.,
2016). In the complex, high dimensional humanoid domain,
we outperform SAC.

3.4 Relationship to Soft Actor-Critic and Soft
Q-Learning
We now show that SAC (Haarnoja et al., 2018; Abdolmaleki
et al., 2018) and the related soft Q-learning, (Haarnoja
et al., 2017) algorithms purportedly derived from MERLIN (Levine, 2018) can be shown to arise from a model
that is closer to VIREL. Consider now the MERLIN lower
bound (Levine, 2018),
















Recall Traces: Backtracking Models for Efficient Reinforcement Learning
Anirudh Goyal, Philemon Brakel, William Fedus, Timothy Lillicrap, Sergey Levine, Hugo Larochelle, Yoshua Bengio
(Submitted on 2 Apr 2018)
In many environments only a tiny subset of all states yield high reward. In these cases, few of the interactions with the environment provide a relevant learning signal. Hence, we may want to preferentially train on those high-reward states and the probable trajectories leading to them. To this end, we advocate for the use of a backtracking model that predicts the preceding states that terminate at a given high-reward state. We can train a model which, starting from a high value state (or one that is estimated to have high value), predicts and sample for which the (state, action)-tuples may have led to that high value state. These traces of (state, action) pairs, which we refer to as Recall Traces, sampled from this backtracking model starting from a high value state, are informative as they terminate in good states, and hence we can use these traces to improve a policy. We provide a variational interpretation for this idea and a practical algorithm in which the backtracking model samples from an approximate posterior distribution over trajectories which lead to large rewards. Our method improves the sample efficiency of both on- and off-policy RL algorithms across several environments and tasks.



refed by infobot




Amplifying the Imitation Effect for Reinforcement Learning of
UCAV’s Mission Execution
Gyeong Taek Lee 1 Chang Ouk Kim 1
Abstract
This paper proposes a new reinforcement learning
(RL) algorithm that enhances exploration by amplifying the imitation effect (AIE). This algorithm
consists of self-imitation learning and random network distillation algorithms. We argue that these
two algorithms complement each other and that
combining these two algorithms can amplify the
imitation effect for exploration. In addition, by
adding an intrinsic penalty reward to the state that
the RL agent frequently visits and using replay
memory for learning the feature state when using an exploration bonus, the proposed approach
leads to deep exploration and deviates from the
current converged policy. We verified the exploration performance of the algorithm through experiments in a two-dimensional grid environment.
In addition, we applied the algorithm to a simulated environment of unmanned combat aerial
vehicle (UCAV) mission execution, and the empirical results show that AIE is very effective for
finding the UCAV’s shortest flight path to avoid
an enemy’s missiles

4. AIE
4.1. Combining SIL and RND
In this section, we explain why combining RND and SIL can amplify the imitation effect and lead to deep exploration. The SIL updates only when the past R is greater than the current Vθ and imitates past decisions. Intuitively, if we combine SIL and RND, we find that the (R − Vθ) value is larger than the SIL because of the exploration bonus. In the process of optimizing the actor-critic network to maximize Rt = Σ∞k=tγk−t(it + et)k, where it is intrin- sic reward and et is extrinsic reward, the increase in it by the predictor network causes R to increase. That is, the learning progresses by weighting the good decisions of the
past. This type of learning thoroughly reviews the learn- ing history.If the policy starts to converge as the learning progresses, the it will be lower for the state that was fre- quently visited. One might think that learning can be slower as (Rt − Vθ) > (Rt+k − Vθ), where k > 0 for the same state and it decreases. However, the SIL exploits past good decisions and leads to deep exploration. By adding an ex- ploration bonus, the agent can further explore novel states. Consequently, the exploration bonus is likely to continue to occur. In addition, using the prioritized experience replay (Schaul et al., 2015), the sampling probability is determined by the (R − Vθ); thus, there is a high probability that the SIL will exploit the previous transition even if it decreases. In other words, the two algorithms are complementary to each other, and the SIL is immune to the phenomenon in which the prediction error (it) no longer occurs.

4.2. Intrinsic Penalty Reward
Adding an exploration bonus to a novel state that the agent visits is clearly an effective exploration method. However, when the policy and predictor networks converge, there is no longer an exploration bonus for the novel state. In other words, the exploration bonus method provides a reward when the agent itself performs an unexpected action, not when the agent is induced to take the unexpected action. Therefore, an exploration method that entices the agent to take unexpected behavior is necessary. We propose a method to provide an intrinsic penalty reward for an action when it frequently visits the same state rather than reward- ing it when the agent makes an unexpected action. The intrinsic penalty reward allows the agent to escape from the converged local policy and helps to experience diverse policies. Specifically, we provide a penalty by transform- ing the current intrinsic reward into λlog(it), where λ is a penalty weight parameter, if the current intrinsic reward is less than the quantile α of the past N intrinsic rewards. This reward mechanism prevents the agent from staying in the same policy. In addition, adding a penalty to the intrinsic reward indirectly amplifies the imitation effect. Since the (Rt − Vθ ) becomes smaller due to the penalty, the probabil- ity of sampling in replay memory is relatively smaller than that of non-penalty transition. SIL updates are more likely to exploit non-penalty transitions. Even if (Rt − Vθ ) < 0 due to a penalty, it does not affect SIL because it is not updated because of the objective of SIL in equation 4. In other words, the intrinsic penalty reward allows the policy network to deviate from the constantly visited state of the agent and indirectly amplifies the imitation effect for the SIL.
4.3. Catastrophic Forgetting in RND
The predictor network in RND mainly learns about the state that the agent recently visited, which is similar to the
catastrophic forgetting of continual task learning that forgets learned knowledge of previous tasks. If the prediction error increases for a state that the agent has visited before, the agent may recognize the previous state as a novel state. Consequently, an agent cannot effectively explore. The method to mitigate this phenomenon is simple but effective. We store the output of the target network and state feature as the memory of the predictor network, just like using a replay memory to reduce the correlation between samples(Mnih et al., 2013), and train the predictor network in a batch mode. Using the predictor memory reduces the prediction error of states that the agent previously visited, which is why the agent is more likely to explore novel states. Even if the agent returns to a past policy, the prediction error of the state visited by the policy is low, intrinsic penalty is given to the state, and the probability of escaping from the state is high.

end




SIL

2
prior
apex--
relatation:
Distributed Importance Sampling A complementary family of techniques for speeding up train- ing is based on variance reduction by means of importance sampling (cf. Hastings, 1970). This has been shown to be useful in the context of neural networks (Hinton, 2007). Sampling non-uniformly from a dataset and weighting updates according to the sampling probability in order to counteract the bias thereby introduced can increase the speed of convergence by reducing the variance of the gradients. One way of doing this is to select samples with probability proportional to the L2 norm of the corresponding gradients. In supervised learning, this approach has been successfully extended to the distributed setting (Alain et al., 2015). An alternative is to rank samples according to their latest known loss value and make the sampling probability a function of the rank rather than of the loss itself (Loshchilov & Hutter, 2015).
Prioritized Experience Replay Experience replay (Lin, 1992) has long been used in reinforce- ment learning to improve data efficiency. It is particularly useful when training neural network function approximators with stochastic gradient descent algorithms, as in Neural Fitted Q-Iteration (Riedmiller, 2005) and Deep Q-Learning (Mnih et al., 2015). Experience replay may also help to prevent overfitting by allowing the agent to learn from data generated by previous versions of the policy. Prioritized experience replay (Schaul et al., 2016) extends classic prioritized sweeping ideas (Moore & Atkeson, 1993) to work with deep neural network function approximators. The approach is strongly related to the importance sampling techniques discussed in the previous section, but us- ing a more general class of biased sampling procedures that focus learning on the most ‘surprising’ experiences. Biased sampling can be particularly helpful in reinforcement learning, since the reward signal may be sparse and the data distribution depends on the agent’s policy. As a result, prioritized experience replay is used in many agents, such as Prioritized Dueling DQN (Wang et al., 2016), UNREAL (Jaderberg et al., 2017), DQfD (Hester et al., 2017), and Rainbow (Hessel et al., 2017). In an ablation study conducted to investigate the relative importance of several algorithmic ingredi- ents (Hessel et al., 2017), prioritization was found to be the most important ingredient contributing to the agent’s performance.

SIL 2
Learning from imperfect demonstrations A few stud- ies have attempted to learn from imperfect demonstrations, such as DQfD (Hester et al., 2018), Q-filter (Nair et al., 2017), and normalized actor-critic (Xu et al., 2018). Our self-imitation learning has a similar flavor in that the agent learns from imperfect demonstrations. However, we treat the agent’s own experiences as demonstrations without us- ing expert demonstrations. Although a similar idea has been discussed for program synthesis (Liang et al., 2016; Abo- lafia et al., 2018), this prior work used classification loss without justification. On the other hand, we propose a new objective, provide a theoretical justification, and systemati- cally investigate how it drives exploration in RL.

与4.1. Entropy-Regularized Reinforcement Learning 
The goal of entropy-regularized RL is to learn a stochastic policy which maximizes the entropy of the policy as well as the γ-discounted sum of rewards (Haarnoja et al., 2017; Ziebart et al., 2008): 
SIL. 这个和sac 一样？
已读
infobot -goal --recall trace---SIL 高reward；也可以是好奇心的rnd的高reward?。rnd-图的-meaning events ；rnd 高reward是否可以作为infobot的goal？



----------------------------

EPISODIC CURIOSITY THROUGH REACHABILITY

step

计算量太大吧？ every step！
用divertity is all you need  改进是不是会很好！！。subgoal skill subgoal ::: stat action stat ;;          subgoal skill subgoal ::: stat action stat ;;





Visual novelty, curiosity, and intrinsic reward in machine learning and the brain
Andrew Jaegle, Vahid Mehrpour, Nicole Rust
(Submitted on 8 Jan 2019)
A strong preference for novelty emerges in infancy and is prevalent across the animal kingdom. When incorporated into reinforcement-based machine learning algorithms, visual novelty can act as an intrinsic reward signal that vastly increases the efficiency of exploration and expedites learning, particularly in situations where external rewards are difficult to obtain. Here we review parallels between recent developments in novelty-driven machine learning algorithms and our understanding of how visual novelty is computed and signaled in the primate brain. We propose that in the visual system, novelty representations are not configured with the principal goal of detecting novel objects, but rather with the broader goal of flexibly generalizing novelty information across different states in the service of driving novelty-based learning.

view invariance
 state invariance: 
One class of recent proposals for novelty-driven RL addressed the view and state invariance challenges by incorporating a method for computing similarity between images. Some of these proposals extend classic count-based proposals by first mapping similar images to the same bin (e.g. using a hash function [17] or by clustering [18]) before counting. A complementary proposal [19] estimated image similarity by training a DNN to estimate the distance in time between pairs of images, motivated by the observation that temporal continuity can capture invariance [20]. Instead of counting how many times states had been visited, this method estimated an image’s novelty by comparing it to familiar images held in a memory buffer.
Another class of proposals for novelty-driven RL used “pseudocounts” to estimate novelty. In contrast to explicit count-based proposals, pseudocount methods address the invariance problems using a model (e.g. a DNN) trained to estimate the probability of images. Pseudocounts are computed based on how the probability of an image changes between the Nth and (N+1)th times it is viewed, where N is often zero (see [21] for the exact expression). Because these methods approximate continuous probabilities, they are well suited to scenarios where the dimensionality is high and hence nearly all counts are zero, but some stimuli are more probable than others. Because pseudocount methods are based on the response after repeated exposure to an image, they bare some similarity to the phenomenon of repetition suppression in the visual system (see below for a discussion of the role of repetition suppression in novelty computation in the brain). Several recent papers have achieved promising results using pseudocounts to drive exploration on difficult RL tasks [21-23].
How does novelty seeking relate to other types of intrinsic motivation? In the case of pseudocount estimates, an important theoretical link has been established between estimates of novelty and the amount of information gain [24] that follows from observing an image [21]. Intuitively, this is because the novelty of an image reflects how much it differs from what we expect to see based on what we’ve seen in the past. Early work on intrinsic motivation established the link between curiosity and measures of image informativeness, such as information gain [25,26]. While the information gained by observing an image cannot be computed directly, several methods have been proposed to approximate it to drive exploration [27,28]. A number of recent papers have also proposed other, related signals to drive exploration, including methods that estimate image informativeness by how variable or
4
unreliable the response to the image is [29], how well the response of a target model can be predicted [30], and by how difficult it is to predict what will follow an image in time [31-33]. Unlike methods for novelty-driven RL, these methods do not estimate novelty explicitly, but they share the goal of driving exploration by estimating the informativeness of images.



Computing and signaling novelty in the primate brain
Our ability to detect visual novelty (or equivalently remember whether we have seen an image) is quite remarkable – for example, we can view thousands of photographs, each only once and each for a few seconds, and then distinguish with high accuracy the specific images that we have already seen from those that remain novel to us [34]. Even after viewing as many as 10,000 distinct photographs, our rates of remembering do not saturate, suggesting that this type of single-exposure visual memory has an exceedingly large capacity [34,35]. The most remarkable aspects of our ability to detect visual novelty are thought to be mediated by our “familiarity” memory system. One effective illustration of familiarity is the experience that we all occasionally have of seeing someone and remembering that we know them but not being able to recall any details about them, at least for a few moments, and this “sense of remembering absent details” is precisely what the familiarity memory system supports. In contrast to recollection-based memories (e.g. of the details about that person, such as their name), which are thought to be largely mediated by the hippocampus, familiarity is thought to be mediated by another brain area in the medial temporal lobe, perirhinal cortex, as well its input from the part of the visual system involved in signaling object and scene information, inferotemporal cortex (IT) [reviewed by 36,37].
How do these brain areas signal visual novelty? Novelty is thought to be signaled in IT and perirhinal cortex via an adaptation-like change in firing rate in response to familiar as compared to novel stimuli, a phenomenon referred to as repetition suppression [38-42]. Consistent with the signatures needed to account for the vast capacity of human single-exposure visual memory behavior, firing rate reductions with familiarity are selective for images, even after viewing large numbers of them, and these response decrements last for several minutes to hours following the single viewing of an image [39,40,42]. These putative visual novelty signals are mixed with signals reflecting visual identity, both within the responses of individual neurons and across the IT population. That is, visual identities of images and their content are thought to be reflected as distinct patterns of spikes across the IT population, and this translates into a population representation in which visual information about the currently-viewed scene is reflected by a population’s vector angle [Fig. 2; reviewed by 43]. In contrast, novelty is thought to be signaled by overall firing rates or equivalently the length of the population response vector, where vectors are longer for novel images and become shorter as they become familiar [42]. Novelty and familiarity modulations are thought to be approximately multiplicative [44,45], which translates to a type of novelty coding for memory that maintains identity vector angle position, thereby preventing the interference of identity and novelty representations [42]. Repetition suppression magnitudes are also continuous and depend on factors such as the time since an image has been viewed, the duration of the viewing, and the number of repeated viewings [reviewed by 46]. This encoding scheme can account for behavior on a familiarity task with a decoder that maps IT neural response to behavior via a simple positively-weighted linear read-out [42].

How is novelty computed by the brain? In the framework described in Figure 2, this amounts to understanding the origin of IT repetition suppression. Repetition suppression is found at all stages of visual processing from the retina to IT, and it strengthens in its magnitude as well as the duration over which it lasts across the visual cortical hierarchy [47]. Consequently, a hierarchical cascade of feed-forward, adaptation-like mechanisms clearly contribute to IT repetition suppression [46]. There are also indications that IT repetition suppression may arise from changes in synaptic weights between recurrently connected units within IT [46,48] and/or feed-back mechanisms from higher brain areas (such as perirhinal cortex) [49,50], although the latter assertion has been the focus of some debate [reviewed by 46].


Highlighted references:
* Tang H, Houthooft R, Foote D, Stooke A, Chen OX, Duan Y, Schulman J, DeTurck F, Abbeel P: #Exploration: A study of count-based exploration for deep reinforcement learning. In Conference on Neural Information Processing Systems (NeurIPS): 2017:2753-2762.
This paper addressed the view and state invariance challenges by adapting count-based methods to image-based RL using hash functions that map images to a relatively small number of bins.
** Bellemare M, Srinivasan S, Ostrovski G, Schaul T, Saxton D, Munos R: Unifying count- based exploration and intrinsic motivation. In Conference on Neural Information Processing Systems (NeurIPS): 2016:1471-1479.
This paper introduced the notion of pseudocounts, which generalize count-based methods for novelty estimation and can be applied to RL problems with high- dimensional, continuous states such as images. The authors formally demonstrated the relationship between pseudocounts and information gain, suggesting that pseudocounts may lead to near-optimal exploration behavior.
* Savinov N, Raichuk A, Marinier R, Vincent D, Pollefeys M, Lillicrap T, Gelly S: Episodic curiosity through reachability. In International Conference on Learning Representations (ICLR): 2019. [19]
This paper computed an intrinsic reward signal that closely resembles a novelty computation using two interesting model components: a learned similarity measure and a memory buffer.
** Meyer T, Rust NC: Single-exposure visual memory judgments are reflected in inferotemporal cortex. eLife 2018, 7:e32259.
This paper demonstrated the plausibility of IT repetition suppression as a novelty signal by illustrating that a positively weighted linear read-out of IT responses could account for remembering and forgetting behavior as a function of time since an image was viewed.
* Hong H, Yamins DL, Majaj NJ, DiCarlo JJ: Explicit information for category-orthogonal object properties increases along the ventral stream. Nat. Neurosci. 2016, 19:613-622.
This paper demonstrated the robust and easily accessible representations of IT populations for properties beyond object identity, including object position.

end


https://spinningup.openai.com/en/latest/spinningup/rl_intro3.html
To actually use this algorithm, we need an expression for the policy gradient which we can numerically compute. This involves two steps: 1) deriving the analytical gradient of policy performance, which turns out to have the form of an expected value, and then 2) forming a sample estimate of that expected value, which can be computed with data from a finite number of agent-environment interaction steps.
where the data must be sampled on the most recent policy.
Taking a step with this gradient pushes up the log-probabilities of each action in proportion to R(\tau), the sum of all rewards ever obtained. But this doesn’t make much sense.
reward-to-go policy gradient,
The most common choice of baseline is the on-policy value function V^{\pi}(s_t). Recall that this is the average return an agent gets if it starts in state s_t and then acts according to policy \pi for the rest of its life.

Empirically, the choice b(s_t) = V^{\pi}(s_t) has the desirable effect of reducing variance in the sample estimate for the policy gradient.
This results in faster and more stable policy learning. It is also appealing from a conceptual angle: it encodes the intuition that if an agent gets what it expected, it should “feel” neutral about it.

Don’t Let the Past Distract You
It turns out that this intuition shows up in the math, and we can show that the policy gradient can also be expressed by
We’ll call this form the “reward-to-go policy gradient,” because the sum of rewards after a point in a trajectory
Implementing Reward-to-Go Policy Gradient

VPG
Exploration vs. Exploitation
VPG trains a stochastic policy in an on-policy way. This means that it explores by sampling actions according to the latest version of its stochastic policy. The amount of randomness in action selection depends on both initial conditions and the training procedure. Over the course of training, the policy typically becomes progressively less random, as the update rule encourages it to exploit rewards that it has already found. This may cause the policy to get trapped in local optima.
https://spinningup.openai.com/en/latest/algorithms/trpo.html
RPO updates policies by taking the largest step possible to improve performance, while satisfying a special constraint on how close the new and old policies are allowed to be. The constraint is expressed in terms of KL-Divergence, a measure of (something like, but not exactly) distance between probability distributions.
