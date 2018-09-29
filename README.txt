Bug2 - Was involved with the send was a differnt MPI_TYPE. The sender tried to send a MPI_INIT but the receiver tried to receive a MPI_FLOAT.
Bug3 - Was there was not inital MPI_INIT or MPI_Finialize.
Bug4 - This can be resolved with MPI_REDUCE
Bug5 - In the send and recive function there was a MPI_BYTE but evey system has a different respresentation of this so we need to use MPI_CHAR because systems use this as one byte
