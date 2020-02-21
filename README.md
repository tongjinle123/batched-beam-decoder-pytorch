# batched-beam-decoder-pytorch
a batched version for beam decode in seq2seq model


init BeamSteper in your decode progress and pass the steper with log_softmax(logit) steper will save current token, current length, current prob in self.token_container self.length_container, self.prob_container
and will raise Error when all beam meet a eos 
still there is a length penalty and best k is saved in self.batch_best_saver 
